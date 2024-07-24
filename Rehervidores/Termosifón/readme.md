# Termosifón vertical

Son generalmente cambiadores de calor de un paso por la coraza y uno por los tubos. El espejo superior de los tubos se coloca cercano al nivel del líquido dentro de la columna. Como se instala cerca de la columna, las pérdidas por fricción por las entradas y salidas del sistema son casi siempre insignificantes. \
Debido a que este tipo de rehervidor debe tener una presión hidrostática capaz de superar las pérdidas por fricción en el sistema. Las pérdidas de fricción son:

+ Por la entrada a la tubería
+ Pérdidas en el rehervidor
+ Pérdidas por el evaporador dentro del rehervidor
+ Presión estática en la columna formada por una mezcla de vapor y de líquido
+ Pérdidas por la salida 

![Termosifón](.../imagen/Termo.PNG)

Por el rehervidor pasa siempre una masa mayor que la quw se va a vaporizar. La relación entre la masa que circula a través del rehervidor a la masa vaporizada recibe el nombre de relación de circulación. Esta relación es casi siempre superior a cuatro y se fija de manera que sea iguales las perdidas de fricción con la columna hidrostática. 

![Columna](../imagen/Colum.PNG)

## **Método de Kern**

### Diferencia de temperaturas

Se supune un $\Delta T$

### **Calor transferido**

$$
Q_g = M \lambda \tag{1} 
$$

Del balance de energía:

$$
Q_{perdido} = Q_{ganado} \tag{2}
$$

$$
Qp = MC_p(\Delta T) \tag{3}
$$

Para calcular las propiedades de los fluidos se usa su temperatura del condensado y vapor.


### **Cálculo del área total de transfrencia de calor**

Se debe calcular el área total de transferencia de calor, puesto que no es posible obtener un valor exacto debido a que no se puede calcular el coeficiente global de energía $U_0$

De la ecuación de diseño:

$$
A_0 = \frac{Q}{U_0 (\Delta T)} \tag{4}
$$

### **Cálculo del número de tubos**

Para determinar el número de tubos para cumplir el área total.

$$
\text{No. tubos} = \frac{A_0}{Ase} \tag{5}
$$

Para conocer el área de tubería es necesario elegir las dimensiones de la tubería, donde:

Espesor de la pared = $x$

Diámetro interno:
$D_i = D_o - 2x$

Área de flujo (tubería):
$A_f = \frac{\pi}{4} D_i^2$

Área superficial:
$A_s = \pi DL$

$D$ = $D_i$ (interna) o $D$ = $D_o$ (externa)

La longitud tiene que ser igual a la altura del líquido en la columna de destilación.

### **Presión hidrostática:**

Se plantea una relación de masa de vapor y líquido (V:L).

Se calcula la masa total y el volumen total:

$$
\text{Masa total} = (ML) + (MV) \tag{6}
$$

$$
\text{Volumen total} = \frac{ML}{\rho_{L}} + \frac{MV}{\rho_{G}} \tag{7} 
$$

Se calcula la densidad de la mezcla vapor-líquido

$$
\rho_{mezcla} = \frac{\text{Masa total}}{\text{Volumen total}} \tag{8}
$$

Presión hidrostática

$$
P = 2.3 \frac{L(\rho_{o}rho_{i}}{\rho_{o} - \rho_{i}} \tag{9}
$$

En donde:

L = longitud
$\rho_i$ = densidad del liquido
$\rho_o$ = densidad de la mezcla

### **Caída de presión**

$$ \text{Area de flujo} = Area de flujo de tuberia * No.Tubos \tag{10}$$

Masa velocidad

$$
G_T = \frac{\text{Masa total}}{\text{Área de flujo} * 3600} \tag{11}
$$

Reynolds en tubería

$$
Re_tubo = \frac{G_{T}Di}{\mu_{L}} \tag{12}
$$

$$
\rho_{media} = \frac{\rho_{L}-\rho_{mezcla}}{ln \frac{\rho_L}{\rho_mezcla}} \tag{13}
$$

**Caída de presión por fricción**

$$
\frac{\Delta P_f}{\rho} = f \frac{G_{T}^{2}L}{2gD_i \rho_{media^{2}}} \tag{13} 
$$

**Caída de presión por vaporización**

$$
\frac{\Delta P_V}{\rho}medio = \frac{G_{T}^{2}}{g \rho_{media}^{2}} \tag{14}
$$

La caída de presión total o resistencia total

$$
\Delta P_T = \Delta P_f + \Delta P_V + P \tag{15}
$$

Fuerza impulzora

$$
F = L * \rho_{L} \tag{16}
$$

La fuerza impulsora tiene que ser parecido a la resistencia total. Si es mayor o menor que la resistencia se tiene que volver a proponer una nueva relación de recirculación.

### **Calculo del coeficiente global de transferencia de energia**

**Cálculo del coeficiente interno de película**

Número de Prandtl

$$
P_r = \frac{C_p \mu}{k} \tag{17}
$$

$k$ = conductividad térmica del fluido condensado
$C_p$ = calor especifíco del fluido condensado
$\mu$ = viscosidad del fluido condensado

Cuando se está en la región turbulenta:

$$
N_u = 0.023 R_e^{0.8} P_r^{0.33} \tag{18}
$$

La relación entre $N_u$ y el coeficiente de película:

$$
N_u = \frac{h_iD_i}{k}
$$

**Calculo del coeficiente externo de película**

Generalmente se usa vapor para calentar por lo tanto solo se escoge un valor del coeficiete.

### **Obtención del coeficiente global de transferencia de calor**

\begin{equation}
U_o = \frac{1}{\frac{D_o}{D_i h_i} + \frac{D_o}{D_ihd_i} + \frac{xD_o}{k_w D_w} + \frac{1}{h d_o} + \frac{1}{h_o}} = \left[ \frac{kcal}{m^2h°C} \right]
\end{equation}

*Donde:*

$D_w = \frac{D_o - D_i}{ln \frac{D_o}{D_i}}$

$k_w$ = conductividad térmica del material del que está construido el tubo

$\frac{D_o}{D_ih_i}$ : Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, al interior de los tubos.

$\frac{D_o}{D_ihD_i}$ : Impedimento al flujo de calor que se da en la capa de suciedad o incrustración al interior del tubo.

$\frac{xD_o}{k_wD_w}$ : Resistencia del material del tubo.

$\frac{1}{hd_o}$ : Flujode calor que existe en la capa de depósitos en el exterior de la tubería.

$\frac{1}{h_o}$ : Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, en el fluido que viaja por la coraza.
