# Método de Bell Delaware

Paso 1. Determinar las temperaturas de entrada y salida del lado de la coraza y de los tubos.

Paso 2. Calcular la diferencia de temperaturas media logarítmica (DMTL):

$$
DMTL = \frac{\Delta T_{1} - \Delta T_{2}}{Ln\frac{\Delta T_{1}}{\Delta T_{2}}} \tag{1}
$$

Sindo

$\Delta T_{1} = T_{1} - t_{2}$

$\Delta T_{2} = T_{2} - t_{1}$

![DMTL](../imagen/DTML.png)

Paso 3. Calcular R y S:

$$
R = \frac{T_{1} - T_{2}}{t_{2} - t_{1}} \tag{2}
$$

$$
S = \frac{t_{2} - t_{1}}{T_{1} - t_{1}} \tag{3}
$$

Para determinar el número de corazas requeridas de tal manera que el factor de corrección de temperatura no sea menor de 0.8.

Paso 4. Determinar la diferencia de temperatura media logarítmica corregida (DTML)_{c}:

$$
DTML_{c} = DMTL \cdot FT \tag{4}
$$

Paso 5. Determinar las temperaturas de bulbo del lado de los tubos y coraza (TbT y TbS):

$$
TbT = \frac{t_{1} + t_{2}}{2} \tag{5}
$$

$$
TbS = \frac{T_{1} + T_{2}}{2} \tag{6}
$$

Paso 6. A la temperatura de bulbo de lado de los tubos, determine las propiedades del fluido:

+ Gravedad específica (SGT)
+ Viscosidad (\mu T), cp
+ Capacidad calorífica (CT), $\frac{BTU}{lb°F}$
+ Conductividad térmica (kT), $\frac{BTU}{hr-ft-°F}$

Paso 7. A la temperatura de bulbo del lado de la coraza, determine las propiedades del fluido:

+ Gravedad específica (SGS)
+ Viscosidad (\mu S), cp
+ Capacidad calorífica (CS), $\frac{BTU}{lb°F}$
+ Conductividad térmica (kS), $\frac{BTU}{hr-ft-°F}$

Paso 8. Determinar los fluidos másicos del lado de la coraza, WS (lb/hr) y del lado de los tubos, WT (lb/hr).

Paso 9. Determinar la carga de calor Q, usando los datos del lado de la coraza o del lado de los tubos.

a. Asumir un valor el coeficiente total de diseño (UD).
b. Calcular el área total (AT):

$$
AT = \frac{Q}{[UD(DTML)_{c}]} \tag{7}
$$

Paso 10. Elegir los siguientes parámetros:

+ Número de pasos por el lado de los tubos (NPT).
+ Longitud de los tubos, (L) ft.
+ Diámetro interior de los tubos, (di) in.
+ Diámetro exterior de los tubos, (do) in.
+ Tipo de arreglo triangular, cuadrado o rotado.
+ Pitch de los tubos, (PT) in.
+ Pitch normal de los tubos, (PN) in.
+ Pitch paralelo, (PP) in.
+ Porciento de corte de la mapara.
+ Número de fajas de sellos (NSS).

Paso 11. Calcular el número de tubos del intercambiador de calor, (NT):

$$
\text{Numero de tubos} = \frac{A}{(\pi(\frac{do}{12})L)} \tag{8}
$$

Se puede modificar la longitud a la longitud a la longitud efectiva, usando L-0.5, en lugar de L, considerando que en promedio se tiene 0.5 pies por los espesores de los espejos, en los dos extremos del intercambiador del calor.

Paso 12. Determinar el área del intercambiador de calor:

$$
A = \pi (\frac{do}{12}L * \text{No. tubos}) \tag{9}
$$

Paso 13. Calcular el coeficiente global de transferencia de calor de diseño, (UD):

$$
UD = \frac{Q}{(NCO(DTML)_{c}A)} \tag{10}
$$

Paso 14. De acuerdo al número total de tubos y al tipo de arreglo, determinar el diámetro exterior de haz de tubos. DOTL (in). 

## Cálculo del coeficiente de película del lado de la coraza.

![Corrección por fugas](./Metodo_Bell_Delaware/correccion_fugas.png)

Paso 15. Determinar el número de hileras cruzadas en una sección transversal (entre los extremos de las mamparas), NC:

$$
NC = \frac{D(1 - (\frac{2LC}{D}))}{PP} \tag{11}
$$

Paso 16. Calcular la fracción de tubos totales en la sección de flujo transversal:

$$
FC = \frac{1}{\pi}(\pi 2(\frac{D-(2LC)}{DOTL}))Sen(Cos^{-1} \frac{D-(2LC)}{DOTL})-2Cos^{1}(\frac{D-(2LC)}{DOTL}) \tag{12}
$$

Donde todos los ángulos están en radianes.

Paso 17. Estimar el número efectivo de hileras en flujo transversal en cada ventana, (NCW):

$$
NCW = \frac{(0.8LC)}{PP} \tag{13}
$$

Esta ecuación asume que el fluido en el lado de la coraza cruzada, en promedio, la mitad de las hileras de tubos en la ventana (cada una de esas hileras dos veces) y que las hileras se extienden 0.8 de la distancia del extremo de la mampara al diámetro interior de la coraza.

Paso 18. Número de mamparas, (NB)

$$
NB = \frac{12L-LSI-LSO}{LS} + 1 \tag{14}
$$

Esta ecuación considera que el espaciamiento de entrada y/o salida entre mamparas puede ser diferente del espaciamiento entre mamparas centrales.

Paso 19. Área de flujo transversal en/o cerca de la línea de centros para una sección de flujo transversal, SM:

Para arreglo cuadrado y cuadrado rotado:
    
$$
SM = LS[D-DOTL+(\frac{DOTL-do}{PN})(PT-do)] \tag{15}
$$

Para arreglo triangular:

$$    
SM = LS[D-DTOL+(\frac{DTOL-do}{PT})(PT-do)] \tag{16}
$$

Paso 20. Calcular la fracción de área de flujo transversal disponible para flujo de "desvio", PSBP estimada de:

$$
FSBP = (\frac{D-DOTL}{SM})LS \tag{17}
$$

Paso 21. Calcular el área de fugas tubo-mampara para una mampara STB, estimada:

$$
STB = 0.3926NT(1 + FC)(2DTB \cdot DO + DTB^{2}) \tag{18}
$$

La construcción tema clase R¨, especifica a DTB de 1/32 pulgadas, donde la longitud máxima de tubo sin soportar (normalmente 2 LS) noexcede 36 pulgadas y DTB de 1/64
pulgadas de otra manera. Los valores deberán ser modificados si se tiene una construcción más ajustada o más holgada, o si se prevee taponamiento por suciedad.

Paso 22. Calcular el ángulo de corte de la mampara,Θ. El ángulo de corte de la mampara es el ángulo subtenidopor la intersección del corte del borde de la mampara con la superficie interior de la coraza. En términos de las cantidades previamente definidas:

$$
\Theta = 2 Cos^-{1} [1-(\frac{2LC}{D})] \tag{19}
$$

Donde el valor del término $COS^{-1}[1 - (\frac{2LC}{D})]$ está en radianes, entre 0 y $\pi/2$

Paso 23. Calcular el área de fugas coraza-mampara para una mampara, SSB. Si el claro dimetral, DSB, es conocido, SSB puede ser calculado:

$$
SSB = \frac{\pi \cdot D \cdot DSB (1 - \theta/2 \pi)}{2} \tag{20}
$$

El valor de DSB se obtiene de la tabla 3 del apéndice. Se deberán considerar tolerancia para construcciones ajustadas u holgadas. En este aspecto, puede notarse que es conservador estimar un claro más grande cuando se calcula la transferencia de calor, en el sentido de calcular un coeficiente de transferencia de calor más bajo del lado decorza. Sin embargo, cuando calculamos la caída de presión se obtiene un estimado conservador (caída de presión más alta) si uno asume claros pequeños.

Paso 24. Calcular el área de flujo a través de la ventana, SW. Esta área es obtenida como la diferencia entre el área total de la ventana, SWG y el área de la ventana ocupada por los tubos, SWT:

$$
SW = SWG - SWT \tag{21}
$$

El valor de SWG puede ser calculado de:

$$
SWG = \frac{D^{2}}{4}[\frac{\theta}{2} - (1 - \frac{2LC}{D}) \cdot Sen(\frac{\theta}{2})] \tag{22}
$$

El área ocupa por los tubos, SWT puede ser calculada de:

$$
SWT = \frac{NT}{S} (1 - FC) \cdot \pi \cdto DO^{2} \tag{23}
$$

Paso 25. Calcular el diámetro equivalente de la ventana, DW (requerido solo si existe flujo laminar, definido como RES ≤ 100), calculado como:

$$
DW = \frac{4SW}{\frac{\pi}{2} \cdot NT \cdot (1 - FC) \cdot DO + D \cdot \theta} \tag{24}
$$

Paso 26. Calcular el número de Reynolds del lado de la coraza, RES. El número de Reynolds de lado de la coraza está definido como:

$$
RES = \frac{12DO \cdot WS}{2.42 \rho S \cdot SM} \tag{25}
$$

Paso 27. Estimar el factor de corrección por efectos de fuga en la mampara, JI, de la fig. 3 del apéndice, para arreglo de tubos dado, usando el valor calculado de RES

Paso 28. Calcular el coeficiente de transferencia de calor para un haz de tubos ideal h0:

$$
hO = JI \cdot CS(\frac{144WS}{SM})(\frac{KS}{CS \cdot  \mu S \cdot 2.42})^{\frac{2}{3}} (\frac{\mu S}{\mu SW})^{0.14} \tag{26}
$$

Paso 29. Determinar el factor de correlación por efectos de configuración de las mamaparas, JC, usando la fig.4 del apéndice o la ecuación siguiente:

$$
JC = FS + 0.524 (1 - FC)^{0.32}(SM/SW)^{0.03} \tag{27}
$$

Este valor es igual a 1.0 para intercambiadores de calor los cuales no hay tubos en la ventana, se incrementa a un valor de 1.15 para un diseño en el cual las ventanas son relativamente pequeñas y la velocidad en la ventana es muy alta, disminuye hasta un valor cerca de 0.52 para cortes de mamparas muy grandes. Un valor típico para un intercambiador de calor bien diseñado es de 1.0.

Paso 30. Calcular el factor de corrección por efectos de fugas en la mampara, JL, usando la fig.5 del apéndice o la ecuación siguiente:

$$
JL = 1 - (1 + \frac{SSB}{STB + SSB} \cdot 0.45 (\frac{STB + SSB}{SM} + 0.1[1 - e^{-30(\frac{STB}{SSB})}])) \tag{28}
$$

Un valor típico de JL se encuentra en el rango de 0.7 a 0.8. JL castiga más las fugas coraza-mampara que las fugas tubo-mampara. La correlación de JL penaliza el diseño de mamparas que se encuentran muy cercanas, que lleva a una fracción excesiva de flujo de fugas, comparado con el flujo transversal.

Paso 31. Estimar el valor del factor de corrección por el flujo que no pasa el haz de tubos, JB. Este factor es determinado en la fig.5 del apéndice como una función de FSBP y de la relación NSS/NC (relación de número de fajas de sello por lado al número de hileras cruzadas en
una sección transversal de flujo) o de la siguiente ecuación:

$$
JB = e^{[-\alpha \cdot FSBP(1 - (\frac{2NSS}{NC})^{\frac{1}{3}})]} \tag{29}
$$

a = 1,5 para flujo laminar y a = 1,35 para flujo en transición o turbulento. JB es el factor de corrección por el flujo que no pasa a través del haz de tubos (corriente C). JB toma en cuenta las diferencias en construcción. Para diferencias relativamente pequeñas entre el diámetro exterior del haz de tubos y el diámetro interior de la coraza, JB = 0.9, y para claros más grandes como los cabezales flotantes removibles JB = 0,7. JB también considera el mejoramiento por las fajas de sello.

Paso 32. Determinar el factor de corrección por gradiente adverso de temperatura a números bajos de Reynolds, JR. Este factor es igual a 1.0 si RES es igual o más grande que 100.

a) si RES < 100, determinar JR∗ de la fig.7 del apéndice, conociendo $NB$ y $NC + NCW$
b) Si RES ≤ 20, JR = JR∗
c) Si 20 < RES < 100, determinar JR de la fig.8 del apéndice conociendo JR∗ y RES.

Paso 33. Calcular el factor de corrección por espaciamiento desigual de mamparas a la entrada o
salida, JS:

$$
JS = \frac{(NB-1) + (LSI/LS)^{(1-n)} + (LSD/LS)^{(1-n)}}{(NB-1) + (LSI/LS) +(LSD/LS)}  \tag{30}
$$

n = 0.6 para flujo turbulento (RES > 100)

n = 1/3 para flujo laminar (RES < 100)

El factor de corrección JS estará usualmente entre 0.85 y 1. Este factor puede ser evaluado
de las figuras 9 y 10.

Paso 34. Calcular el coeficiente de película del lado de la coraza, usando la ecuación:

$$
HO = hO \cdot JC \cdot JL \cdot JB \cdot JR \cdot JS \tag{31}
$$

## **Cálculo del coeficiente de película del lado de los tubos**

Paso 35. Calcular el área del flujo en los tubos, AT:

$$
AT = (\pi \cdot \frac{DI^{2}}{AT}) \frac{NT}{144 NPT} \tag{32} 
$$

Paso 36. Determinar el gasto másico en los tubos, GT:

$$
GT = \frac{WT}{AT} \tag{33}
$$

Paso 37. Calcular la velocidad del lado de los tubos, VT:

$$
VT = \frac{GT}{3600 \cdot SGT \cdot 62.37} \tag{34}
$$

Paso 38. Determinar el número de Reynolds del lado de los tubos, RET:

$$
RET = \frac{GT \cdot DI}{12 \cdot \mu T \cdot 2.42} \tag{35}
$$

Paso 39. Calcular el coeficiente de película del lado de los tubos, HIO:

+ Para agua:

$$
HIO = (\frac{150}{DI^{0.2}})[1 + (\frac{0.011(t_{1}+t_{2})}{2})] \cdot VT^{0.8} (\frac{DI}{DO}) \tag{36}
$$

+ Para otros fluidos:

$$
HIO = 0.027 RET^{0.796} (\frac{2.42 \cdot CT \cdot \mu T}{KT})^{\frac{1}{3}} (\frac{12KT}{DI}) (\frc{DI}{DO}) \tag{37}
$$

Paso 40. Estimar la temperatura de pared, tW:

+ Para fluido caliente en la coraza

$$
tW = [\frac{t_{1} + t_{2}}{2}] + [\frac{HO}{HIO + HO}][\frac{T_{1} + T_{2}}{2} - \frac{t_{1} + t_{2}}{2}] \tag{38}
$$

+ Para fluido caliente por el lado de los tubos

$$
tW = [\frac{t_{1} + t_{2}}{2}] + [\frac{HIO}{HIO + HO}][\frac{T_{1} + T_{2}}{2} - \frac{t_{1} + t_{2}}{2}] \tag{39}
$$

## **Cálculo de la caída de presión del lado de la coraza**

Paso 41. Determinar el factor de fricción, FSI, con el valor calculado de RES, usando la fig.11 del apéndice para arreglo triangular y arreglo cuadrado rotado y la fig.12 del apéndice para arreglo cuadrado.

Paso 42. Calcular la caída de presión para una sección de flujo transversal ideal, $\Delta PBI$:

$$
\Delta PBI = {0.69 \times 10^{-6} \cdot FSI \cdot WS^{2} \cdot NC}{SM^{2} \cdot 62.37 \cdot SGS} (\frac{\mu SW}{\rho S}) 0.14 \tag{40}
$$

Paso 43. Calcular la caída de presión para una sección de ventana ideal, $\Delta PWI$:

Si $RES \geq 100$:

$$
\Delta PWI = \frac{WS^{2}(2+0.6\cdot NCW) 1.73\times 10^{-7}}{SM\cdot SW \cdot SGS \cdot 62.37} \tag{41}
$$

Si $RES < 100$:

$$
\Delta PWI = \frac{0.75\times 10^{-6} \cdot \mu S \cdot WS}{SM \cdot SW \cdot SGS \cdot 62.37}[\frac{NCW}{PT-Do}+\frac{LS}{DW^{2}}] + \frac{WS^{2} \cdot 0.345\times 10^{-6}}{SM \cdot SW \cdot SGS \cdot 62.37} \tag{42}
$$

Paso 44. Determinar el factor de corrección por el flujo que no pasa el haz de tubos, RB de la fig. 13 del apéndice como una función de FSBP y NSS/NC. Este factor es diferente en magnitud a JB, pero similar en forma. El valor de RB va de 0.5 a 0.8, dependiendo del tipo de construcción y el número de gajos o fajas de sello.

Paso 45. Determinar el factor de corrección por efecto de fugas en la mampara para la caída de presión, RL. Este valor se obtiene de la fig. 14 del apéndice.

Paso 46. Calcular el factor de corrección por espaciamiento desigual entre mamparas, RS. Las ecuaciones

$$
RS = \frac{1}{2} ((\frac{LSI}{LS})^{-n} + (\frac{LSD}{LS})) \tag{43}
$$

$n = 1.6$ para un flujo turbulento (RES > 100)

$n = 1.0$ para un flujo laminar (RES < 100)

Paso 47. Determinar la caída de presión a través del lado de la coraza (excluyendo boquillas). $\Delta PS$:

$$
\Delta PS = [(NB-1)\Delta PBI \cdot RB + NB \cdot \Delta PWI]\cdot RL + [2 \Delta PBI \cdot RB (1 + \frac{NCW}{NC}) RS] \tag{44}
$$

## **Cálculo de la caída de presión del lado de tubo**

Paso 48. Calcular la caída de presión para tramos rectos:

$$
\Delta PTT = \frac{0.00273 \cdot RET^{-0.24895} \cdot GT^{2}\cdot L \cdot NPT \cdot 12}{(5.22 \times 10^{10} \cdot dI \cdot SGT)(\frac{\frac{\mu T}{\mu WT}})^{0.14}} \tag{45}
$$

Paso 49. Cacular la caída de presión para retornos, $\Delta PR_{1}$:

$$
\Delta PR_{1} = \frac{4 GT^{2.0015} \cdot 1.34248 \times 10^{-13} \cdot NPT}{SGT} \tag{46}
$$


Paso 50. Calcular la caída de presión total del lado de los tubos, $\Delta PT$:

$$
\Delta PT = \Delta PTT + \Delta PR \tag{47}
$$

## **Cálculo del área real**

Paso 51. Calcular la caída del coeficiente global de transferencia de calor limpio, UC:

$$
UC = \frac{HO \cdot HIO}{HO + HIO} \tag{48}
$$


Paso 52. Calcular el coeficiente global de transferencia de calor de servicio $U_{O}$, basado en el área de transferencia de calor del lado de la coraza:

$$
U_{O} = \frac{1}{[(\frac{1}{HIO}) + (\frac{1}{HO}) + RIO + RO]} \tag{49}
$$


Paso 53. Calcular el área requerida:

$$
A_{O} = \frac{Q}{U_{O}(DMTL)_{c}} \tag{50}
$$

Paso 54. Calcular el porciento de sobrediseño

$$
SD = (\frac{A}{A0} - 1) \cdot 100 \tag{51}
$$