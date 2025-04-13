
# Modelamiento de sistemas mecanicos rotacionales

El modelamiento de sistemas rotacionales consiste en representar matemáticamente el comportamiento dinámico de elementos que giran alrededor de un eje. Estos sistemas se encuentran en motores, engranajes, turbinas y muchos mecanismos mecánicos.

Para modelarlos se aplica la segunda ley de Newton en forma rotacional, también conocida como la ley del momento:

$\sum \tau = J \alpha$

donde 
𝜏
τ es el torque neto, 
𝐽
J es el momento de inercia y 
𝛼
α es la aceleración angular.

En estos sistemas se analizan elementos como discos, poleas, ejes y componentes que introducen resistencia al giro como fricción rotacional y resortes torsionales. Al igual que en sistemas traslacionales, pueden representarse mediante ecuaciones diferenciales, y su comportamiento puede estudiarse usando herramientas como la transformada de Laplace para obtener funciones de transferencia.


## 1. Introduccion

Introduccion a modelamiento de sistemas mecanico rotacionales

## 2. Aplicaciones típicas
Sistemas de suspensión automotriz (con masas representando ruedas y carrocería).

Estructuras de edificios ante sismos (pisos representados como masas).

Sistemas robóticos de múltiples grados de libertad.






# ⚙️ Modelamiento de Sistemas Rotacionales

El **modelamiento de sistemas rotacionales** consiste en representar el comportamiento dinámico de cuerpos en rotación aplicando la forma rotacional de la segunda ley de Newton:

```math
\sum \tau = J \alpha
```

Donde:

- \( \sum \tau \): suma de torques (N·m)  
- \( J \): momento de inercia (kg·m²)  
- \( \alpha \): aceleración angular (rad/s²)  

También se utilizan otros elementos como:

- **Resorte torsional**:  
  ```math
  \tau = K_\theta \theta
  ```
  
- **Amortiguador rotacional**:  
  ```math
  \tau = B_\theta \dot{\theta}
  ```

---

## 🗝️ Definiciones Clave

| Término                    | Definición                                                                 |
|---------------------------|----------------------------------------------------------------------------|
| **Torque ( \( \tau \) )**        | Fuerza de giro aplicada a un eje. Se mide en Newton-metros (N·m).            |
| **Momento de inercia ( \( J \) )** | Resistencia del cuerpo a cambiar su velocidad angular.                        |
| **Velocidad angular ( \( \omega \) )** | Tasa de cambio de la posición angular. Medida en rad/s.                      |
| **Aceleración angular ( \( \alpha \) )** | Derivada de la velocidad angular respecto al tiempo.                         |
| **Resorte torsional**      | Elemento que aplica torque proporcional al ángulo de giro.                 |
| **Amortiguador rotacional**| Componente que genera torque resistivo proporcional a la velocidad angular.|
| **Sistema rotacional**     | Sistema donde los componentes giran en torno a un eje fijo.                |

---

## 🛠️ Aplicaciones de Sistemas Rotacionales

1. **Motores eléctricos y generadores**  
   - Conversión de energía eléctrica ↔ mecánica.  
   - Modelado del rotor con torque, fricción y momento de inercia.

2. **Sistemas de transmisión (engranajes, poleas)**  
   - Análisis del movimiento rotacional transferido entre ejes.

3. **Robótica**  
   - Control de servomotores y actuadores rotacionales precisos.

4. **Automóviles**  
   - Modelado del cigüeñal, sistema de frenos, y control ABS.

5. **Turbinas y hélices**  
   - Predicción de arranque, régimen estable y freno dinámico.

6. **Instrumentación rotacional (giroscopios)**  
   - Estabilización en drones, naves y satélites.
##4. Sistemas mecanicos acoplados y verticales

Los elementos básicos de todo sistema mecánico son la masa, el resorte y el amortiguador. El estudio del movimiento en sistemas mecánicos se corresponde con el análisis de sistemas dinámicos.

### 4.1 sistemas verticales 

En los sistemas verticales, la dirección del movimiento es afectada por la gravedad, lo cual modifica el equilibrio estático del sistema. En este caso, las ecuaciones diferenciales incluyen el peso de las masas (
𝑚
𝑔
mg) como parte de las fuerzas externas. Sin embargo, si se considera el análisis respecto a la posición de equilibrio, el término gravitacional se puede eliminar, simplificando el análisis dinámico.

![Logo](https://masam.cuautitlan.unam.mx/dycme/dsf/wp-content/uploads/sites/11/2021/07/masaresamor.svg)


Figura 1. sistemas verticales 

### 4.2 sistemas acoplados
El modelamiento de sistemas acoplados consiste en representar y analizar sistemas mecánicos en los que dos o más elementos (como masas) están conectados de forma que el movimiento de uno influye en el otro. Estas conexiones se dan a través de resortes, amortiguadores u otros elementos, y el objetivo es describir el sistema mediante ecuaciones diferenciales que predicen su comportamiento dinámico.



Figura 2.  sistemas acoplados


 ## 6. Ejercicios 
 
 📚 Hallar la funcion de transferencia 

![Logo]()

Figura 3. sistema masa resorte amortiguador amortiguador


### Ley de newton

### Ecuación para la masa m1

$m_1 \ddot{x}_1 + (b_1 + b_2) \dot{x}_1 + (k_1 + k_2) x_1 - b_2 \dot{x}_2 - k_2 x_2 = u(t)$

### Ecuación para la masa m2

$m_2 \ddot{x}_2 + b_2 \dot{x}_2 + k_2 x_2 - b_2 \dot{x}_1 - k_2 x_1 = 0$

 📚 Hallar la funcion de transferencia 

![Logo](https://virtual.cuautitlan.unam.mx/intar/ime/wp-content/uploads/sites/15/2021/06/Sist2Orden.jpg)

### Ley de newton

% Ecuación diferencial del sistema
$M \ddot{x}(t) + B \dot{x}(t) + K x(t) = f(t)$


 ## 6. Conclusion

El modelamiento de sistemas acoplados y verticales permite analizar cómo interactúan múltiples componentes mecánicos, considerando fuerzas como resortes, amortiguadores y gravedad. A través de ecuaciones diferenciales y técnicas como la transformada de Laplace, se puede predecir y controlar el comportamiento dinámico del sistema. Esta herramienta es clave en el diseño de estructuras, máquinas y sistemas de control.

 ## 7. Referencias


 
