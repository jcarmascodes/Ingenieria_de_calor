# **Condensadores**

### **Calor transferido**

Ecuación de diseño:

$$
Q = U_0 A_0 (\Delta T_{lm}) \tag{1}
$$

Del balance de energía:

$$
Q_{perdido} = Q_{ganado} \tag{2}
$$

$$
Q = MC_p(\Delta T) \tag{3}
$$

Para calcular las propiedades de los fluidos se usa su temperatura media $T_m$

$$
T_m = \frac{T_1+T_2}{2} \tag{3}
$$

<h4> Del balance de energía se cuando no existe cambido de estado </h4>

$$
Q_{ganado} = M_{x}C_{px}(T_1 - T_2) \tag{4}
$$

$$
Q_{perdido} = M_{vapor}C_{px}(H_{V} - H_{L}) \tag{5}
$$

Donde:

$H_{V}$ = Entalpía del vapor

$H_{L}$ = Entalpía del condensado

### **Cálculo de diferencia de temperatura logarítmica media** 

$$
\Delta T_{lm} = \frac{\Delta T_1 - \Delta T_2}{ln \frac{\Delta T_1}{\Delta T_2}} \tag{6}
$$

Donde:

$$
\Delta T_1 = T_1 - t_2
$$

$$
\Delta T_2 = T_2 - t_1
$$

### **Cálculo del área total de transfrencia de calor**

Se debe calcular el área total de transferencia de calor, puesto que no es posible obtener un valor exacto debido a que no se puede calcular el coeficiente global de energía $U_0$. De la ecuación de diseño:

$$
A_0 = \frac{Q}{U_0 (\Delta T_{lm})F} \tag{7}
$$

### **Cálculo del número de tubos**

Para determinar el número de tubos para cumplir el área total, se debe proponer la velocidad que lleva el fluido al interior de los tubos. Debe ser mayor a la mínima recomendada ($1 \frac{m}{s}$).

Entonces la velocidad propuesta es: $1 \frac{m}{s}$

$$
\text{Área de flujo fluido} = \frac{\text{flujo volumétrico}}{\text{Velocidad del fluido}} \tag{8}
$$

$$
\text{No. tubos} = \frac{\text{Área de flujo (fluido)}}{\text{Área de flujo (tubería)}} \tag{9}
$$

Para conocer el área de flujo de tubería es necesario elegir las dimensiones de la tubería, donde:

Espesor de la pared = $x$

Diámetro interno:
$D_i = D_o - 2x \tag{10}$ 

Área de flujo (tubería):
$A_f = \frac{\pi}{4} D_i^2 \tag{11}$

Área superficial:
$A_s = \pi DL \tag{12}$

$D$ = $D_i$ (interna) o $D$ = $D_o$ (externa)

Ya que se conoce el No. de tubos, es necesario determinar la longitud:

Diámetro interno:

$$
A_0 = A_{se}(\text{No. tubos})L \tag{13}
$$

### **Cálculo del número de pasos:**

$$
\text{No. pasos} = \frac{L}{\text{Longitud deseada del intercambiador}} \tag{14}
$$

$$
\text{No. total de tubos} = ({\text{No.tubos}})({\text{No.pasos}}) \tag{15}
$$

### **Calculo del coeficiente global de transferencia de energia**

#### **Cálculo del coeficiente interno de película**

Área de flujo por paso:

$$
\text{Af por paso} = D_i^2 \frac{\pi}{4}{\text{No. tubos por paso}} \tag{16}
$$

$$
\text{No. tubos por paso} = \frac{\text{No. total de tubos}}{\text{No. paso}} \tag{17}
$$

$$
V_{real} = \frac{\text{flujo volumétrico}}{\text{Af por paso}} \tag{18}
$$

$$
R_e = \frac{D_i V \rho}{\mu} \tag{19}
$$

Cuando se está en la región turbulenta, donde se tienen las siguientes ecuaciones:

Número de Prandtl
$$
P_r = \frac{C_p \mu}{k} \tag{20}
$$

$k$ = conductividad térmica del fluido

$$
N_u = 0.023 R_e^{0.8} P_r^{0.4} \tag{21}
$$

La relación entre $N_u$ y el coeficiente de película:
$$
N_u = \frac{h_iD_i}{k} \tag{22}
$$

Reordenando para el coeficiente de película:

$$
h_{i} = \frac{N_{u}k}{D_{i}} \tag{23}
$$

#### **Calculo del coeficiente externo de película**

El caluculo del coeficiente externo de película puede ser estimada a partir de los rangos que se muestran en el apéndice O. Por lo tanto, el cálculo no se vuelve muy importante o necesario, ya que a valores tan elevado del coeficiente, no ofrecen una importante resistencia al flujo de calor.

En caso que la condensación no se lleve a cabo con vapor de agua, sino con otra sustancia o mezclas, se vuelve indispensable del calculo del coeficiente externo.

Si la condensación se da sobre tubos horizontales (solamente una hilera de tubos), entonces:

$$
\frac{h_o D_o}{k} = 0.73 (\frac{D_o^3 \rho^2 g \lambda}{k \mu \Delta T})^{1/4} = 0.76 (\frac{D_o^3 \rho^2 g}{\mu \Gamma})^{1/3} \tag{24}
$$

Donde:

$g$ = Aceleración de la gravedad

$\rho$ = Densidad del condensado

$\mu$ = Viscosidad del condensado

$k$ = Conductividad térmica del condensado

$\lambda (\Delta H)$ = Calor latente del condensado

$\Delta T = T_v - T_s$

$T_v$ = Temperatura del vapor

$T_s$ = Temperatura de la pared del tubo

$\Gamma$ = Masa del condensado por unidad de superficie ($\frac{W}{\pi D}$)

$W$ = Masa de condensado por tiempo y tubo

Como se puede observar, las propiedades físicas involucradas en el cálculo del coeficiente de película son las del condensado, y éstas se obtienen a la temperatura de película.

$$
T_f = T_v - \frac{3}{4} (T_v-T_s) \tag{25}
$$

Si se desea calcular el coeficiente de película externo en un haz de tubos, es necesario tomar en cuenta el número de tubos que se encuentran uno encima de otro. La ecuación utilizada para este fin es similar a la usada en condensación sobre tubos horizontales, la diferencia es que ahora se toma en cuenta el número de tubos que se encuentran encima o por debajo.

$$
\frac{h_o D_o}{k} = 0.73(\frac{D_o^2 \rho^2 g \lambda}{k \mu \Delta T N})^\frac{1}{4} \tag{26}
$$

Donde:

$N$ = Número de tubos que están uno ensima de otro en una hilera

Cuando se maneja vapor de agua a presión atmosférica puede utilizarse la siguiente ecuación.

$$
h_o = \frac{9235}{D_o^{1/4} \Delta T^{1/3}} \tag{27} 
$$

Donde:

$\Delta T = \frac{T_v - T_s}{2} \tag{28}$

### **Obtención del coeficiente global de transferencia de calor**

$$
U_o = \frac{1}{\frac{D_o}{D_i h_i} + \frac{D_o}{D_ihd_i} + \frac{xD_o}{k_w D_w} + \frac{1}{h d_o} + \frac{1}{h_o}} = \left[ \frac{kcal}{m^2h°C} \right] \tag{29}
$$

*Donde:*

$D_w = \frac{D_o - D_i}{ln \frac{D_o}{D_i}} \tag{30}$

$k_w$ = conductividad térmica del material del que está construido el tubo

$\frac{D_o}{D_ih_i} \tag{31}$
Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, al interior de los tubos.

$\frac{D_o}{D_ihD_i} \tag{32}$
Impedimento al flujo de calor que se da en la capa de suciedad o incrustración al interior del tubo.

$\frac{xD_o}{k_wD_w} \tag{33}$ 
Resistencia del material del tubo.

$\frac{1}{hd_o}$ 
Flujo de calor que existe en la capa de depósitos en el exterior de la tubería.

$\frac{1}{h_o} \tag{34}$
Resistencia al flujo de calor que existe en el fluido, desde la zona de turbulencia hasta la zona laminar, en el fluido que viaja por la coraza.


### **Caída de presión**

#### **Caída de presión en los tubos**
$$
\frac{\Delta P_L}{\rho} = F_D \frac{V_{real}^2LN_{pasos}}{2gD_i}  \tag{35}
$$

$$
\frac{\Delta P_r}{\rho} = 4N_{pasos} \frac{V_{real}^2}{2g}  \tag{36}
$$

$$
\Delta P_T = \Delta P_L + \Delta P_r = \left[ \frac{kg}{cm^2} \right] \tag{37}
$$

**Para condensación en tubos**

$$
\frac{\Delta P}{\rho} = \frac{F_{D} G_{T}{2} L}{4gDi \rho^{2}} \tag{38}
$$

#### **Caída de presión en la coraza**
$$
\frac{\Delta P_s}{\rho} = \frac{1}{2} F_s \frac{G_s^2D_s(n+1)}{2gD_e \rho ^2}  \tag{39}
$$
