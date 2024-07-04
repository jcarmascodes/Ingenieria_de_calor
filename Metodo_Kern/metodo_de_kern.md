# Fundamento Teórico

Los equipos de transferencia de calor son equipos destinados a transferir calor de un fluido a otro, de forma controlada separados por una pared.

El intercambiador de tubos y coraza es el equipo más común en la industrisa de procesos, se usan para servicios en los que se requieren grandes superficies de intercabio. Estos intercambiadores de calor consisten en una cantidad de tubos empacado en una coraza.

![](https://static.wixstatic.com/media/e88453_b1f5db218ff7407abaf7ec9f62d7a709~mv2.png/v1/fill/w_640,h_284,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/e88453_b1f5db218ff7407abaf7ec9f62d7a709~mv2.png)

El método de Kern fue propuesto en 1950, es el primer método de cálculo de un intercambiador sistematizado.

[Ejemplo](../Ejemplo.ipynb)

## Formulas

### **Calor transferido**

Ecuación de diseño:

$$
Q = U_{0} A_{0} (\Delta T_{lm})F \tag{1}
$$

Del balance de energía:

$$
Q_{perdido} = Q_{ganado} \tag{2}
$$

$$
Q = MC_{p}(\Delta T) \tag{3}
$$

Para calcular las propiedades de los fluidos se usa su temperatura media $T_m$

$$
T_{m} = \frac{T_1+T_2}{2} \tag{4}
$$

<h4> Del balance de energía se calcula el calor transferido </h4>

$$
Q_{perdido} = M_{benceno}C_{pbenceno}(T_{1} - T_{2}) \tag{5}
$$

$$
Q_{ganado} = M_{o-xileno}C_{po-xileno}(t_{2} - t_{1}) \tag{6}
$$

### **Cálculo de diferencia de temperatura logarítmica media** 

$$
\Delta T_{lm} = \frac{\Delta T_{1} - \Delta T_{2}}{ln \frac{\Delta T_{1}}{\Delta T_{2}}} \tag{7}
$$

$$
\Delta T_{1} = T_{1} - t_{2} \tag{8}
$$

$$
\Delta T_{2} = T_{2} - t_{1} \tag{9}
$$

### **Cálculo del área total de transfrencia de calor**

Se debe calcular el área total de transferencia de calor, puesto que no es posible obtener un valor exacto debido a que no se puede calcular el coeficiente global de energía $U_{0}$. De la ecuación de diseño:

$$
A_{0} = \frac{Q}{U_{0} (\Delta T_{lm})F} \tag{10}
$$

### **Cálculo del número de tubos**

Para determinar el número de tubos para cumplir el área total, se debe proponer la velocidad que lleva el fluido al interior de los tubos. Debe ser mayor a la mínima recomendada ($1 \frac{m}{s}$).

Entonces la velocidad propuesta es: $1 \frac{m}{s}$

$$
\text{Área de flujo fluido} = \frac{\text{flujo volumétrico}}{\text{Velocidad del fluido}} \tag{11}
$$

$$
\text{No. tubos} = \frac{\text{Área de flujo (fluido)}}{\text{Área de flujo (tubería)}} \tag{12}
$$

Para conocer el área de flujo de tubería es necesario elegir las dimensiones de la tubería, donde:

Espesor de la pared = $x$

Diámetro interno:
$D_{i} = D_{o} - 2x \tag{13}$ 

Área de flujo (tubería):
$A_{f} = \frac{\pi}{4} D_i^{2} \tag{14}$

Área superficial:
$A_{s} = \pi DL \tag{15}$

$D$ = $D_i$ (interna) o $D$ = $D_o$ (externa)

Ya que se conoce el No. de tubos, es necesario determinar la longitud:
Diámetro interno:

$$
A_{0} = A_{se}(\text{No. tubos})L \tag{16}
$$

### **Cálculo del número de pasos:**

$$
\text{No. pasos} = \frac{L}{\text{Longitud deseada del intercambiador}} \tag{17}
$$

$$
\text{No. total de tubos} = ({\text{No.tubos}})({\text{No.pasos}}) \tag{18}
$$

### **Calculo del coeficiente global de transferencia de energia**

**Cálculo del coeficiente interno de película**

Área de flujo por paso:

$$
\text{Af por paso} = D_i^2 \frac{\pi}{4}{\text{No. tubos por paso}} \tag{19}
$$

$$
\text{No. tubos por paso} = \frac{\text{No. total de tubos}}{\text{No. paso}} \tag{20}
$$

$$
V_{real} = \frac{\text{flujo volumétrico}}{\text{Af por paso}} \tag{21}
$$

$$
R_{e} = \frac{D_{i} V \rho}{\mu} \tag{22}
$$

Cuando se está en la región turbulenta, donde se tienen las siguientes ecuaciones:

Fluido que se entría:

$$
N_{u} = 0.023 R_{e}^{0.8} P_{r}^{0.3} \tag{23}
$$

La relación entre $N_u$ y el coeficiente de película:

$$
N_{u} = \frac{h_{i}D_{i}}{k} \tag{24}
$$

Número de Prandtl:

$$
P_{r} = \frac{C_{p} \mu}{k} \tag{25}
$$

$k$ = conductividad térmica del fluido

**Calculo del coeficiente externo de película**

$$
\frac{h_{o} D_{o}}{k} = 0.36 \left( \frac{D_{e}G_{s}}{\mu} \right)^{0.55} (P_{r})^{0.33} \left( \frac{\mu}{\mu_{s}} \right)^{0.14} \tag{26}
$$

$$
h_{o} = \left[ \frac{kcal}{m^2h°C} \right] \tag{27}
$$

Diámetro equivalente para arreglo cuadrangular:

$$
D_{e} = \frac{4(P_{t}^2 - \frac{\pi D_{o}^2}{4})}{\pi D_{o}} = [m] \tag{28}
$$

Masa velocidad:

$$
G_{s} = \frac{\text{flujo másico}}{as} \tag{29}
$$

Área de flujo en los tubos:

$$
as = \frac{D_{s}CB}{P_{t}} \tag{30}
$$

$D_s$ = Diámetro interno de la coraza,
$C$ = Claro entre tubos,
$B$ = Distancia entre baffles,
$Pt$ Distancia de centro a centro entre los tubos (pitch)

$$
C = P_{t} - D_{o} \tag{31}
$$

$$
B = \frac{D_{s}}{5} \tag{32}
$$

### **Obtención del coeficiente global de transferencia de calor**

$$
U_{o} = \frac{1}{\frac{D_{o}}{D_{i} h_{i}} + \frac{D_{o}}{D_{i}hd_{i}} + \frac{xD_{o}}{k_{w} D_{w}} + \frac{1}{h d_{o}} + \frac{1}{h_{o}}} = \left[ \frac{kcal}{m^2h°C} \right] \tag{33}
$$

*Donde:*

$D_{w} = \frac{D_{o} - D_{i}}{ln \frac{D_{o}}{D_{i}}}$

$k_{w}$ = conductividad térmica del material del que está construido el tubo

$\frac{D_{o}}{D_{i}h_{i}}$ : Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, al interior de los tubos.

$\frac{D_{o}}{D_{i}hD_{i}}$ : Impedimento al flujo de calor que se da en la capa de suciedad o incrustración al interior del tubo.

$\frac{xD_{o}}{k_{w}D_{w}}$ : Resistencia del material del tubo.

$\frac{1}{hd_{o}}$ : Flujode calor que existe en la capa de depósitos en el exterior de la tubería.

$\frac{1}{h_{o}}$ : Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, en el fluido que viaja por la coraza.

### **Caída de presión**

**Caída de presión en los tubos**

$$
\frac{\Delta P_{L}}{\rho} = F_{D} \frac{V_{real}^2LN_{pasos}}{2gD_{i}} = [m] \tag{34}
$$

$$
\frac{\Delta P_{r}}{\rho} = 4N_{pasos} \frac{V_{real}^2}{2g} = [m] \tag{35}
$$

$$
\Delta P_{T} = \Delta P_{L} + \Delta P_{r} = \left[ \frac{kg}{cm^2} \right] \tag{36}
$$

**Caída de presión en la coraza**

$$
\frac{\Delta P_{s}}{\rho} = F_{s} \frac{G_{s}^2 D_{s}(n+1)}{2gD_{e} \rho ^2} = [m] \tag{37}
$$
