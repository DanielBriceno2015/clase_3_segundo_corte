

## 1. Introduccion






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
## Intriduccion


El modelamiento de sistemas rotacionales consiste en representar matemáticamente el comportamiento dinámico de elementos que giran alrededor de un eje. Estos sistemas se encuentran en motores, engranajes, turbinas y muchos mecanismos mecánicos.

![Logo](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhRtNrHyDJxaA0RKyaJnNmrNu425mD9-8XlrXkkKXmLALvVcdw7F07l2Mfq7lmMAP2ki_PYZcHu0yw-K2dK37nWK4b0GUyHnGUYUdWnHz1Qsr2mV-Qam8RFcDR_IgKGY4OmRj_RKs8NPA/s200/trans.png)


Figura 1. modelamiento de sistemas rotacionales


## 🔑  Definiciones Clave

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

 ## 6. Ejercicios 
 
 📚 Hallar la funcion de transferencia 

![Logo](https://www.researchgate.net/profile/I-Canton/publication/337893922/figure/fig4/AS:834920016523269@1576071852626/Figura-33-Sistema-rotacional-masa-resorte-amortiguador.jpg)


Este modelo representa un **sistema rotacional** compuesto por:

- Un **resorte torsional** con constante de rigidez \( k \)
- Un **amortiguador rotacional** con coeficiente de fricción \( b \)
- Un **momento de inercia** \( J \)
- Una **entrada de torque** \( \tau(t) \)
- Una **salida angular** \( \theta(t) \)

---

### Ecuaciones del Sistema

Aplicamos la segunda ley de Newton para sistemas rotacionales:

```math
\sum \tau = J \ddot{\theta}(t)
```

Las fuerzas internas del sistema son:

- Torque del resorte:  
  ```math
  \tau_k = -k \theta(t)
  ```

- Torque del amortiguador:  
  ```math
  \tau_b = -b \dot{\theta}(t)
  ```

Sustituyendo en la ecuación de movimiento:

```math
\tau(t) - b \dot{\theta}(t) - k \theta(t) = J \ddot{\theta}(t)
```

---

### Función de Transferencia

Aplicando la **transformada de Laplace** con condiciones iniciales cero:

```math
\tau(s) - b s \Theta(s) - k \Theta(s) = J s^2 \Theta(s)
```

Factorizando:

```math
\tau(s) = \Theta(s) (J s^2 + b s + k)
```

Finalmente, la **función de transferencia** del sistema es:

```math
\frac{\Theta(s)}{\tau(s)} = \frac{1}{J s^2 + b s + k}
```

---


 📚 Hallar la funcion de transferencia 

![Logo](https://ocw.ehu.eus/file.php/83/cap31_html/cap315x.png)

 Relación entre número de dientes y radios

$r_1 N_2 = r_2 N_1$

 Relación entre desplazamientos angulares y radios

$\theta_1 r_1 = \theta_2 r_2$

Relación entre torques cuando no hay pérdidas

$T_1 \theta_1 = T_2 \theta_2$



 ## 6. Conclusion

El modelamiento de sistemas rotacionales permite representar dinámicamente componentes mecánicos como discos, engranajes y motores, facilitando su análisis y control. A través de ecuaciones diferenciales y funciones de transferencia, se puede predecir su comportamiento ante diferentes entradas. Estos modelos son fundamentales en la ingeniería para diseñar sistemas eficientes, precisos y seguros en aplicaciones como robótica, automatización y sistemas mecatrónicos.

 ## 7. Referencias

 
Universidad del País Vasco. (s.f.). Capítulo 3: El modelo keynesiano I. OpenCourseWare UPV/EHU. Recuperado el 13 de abril de 2025, de https://ocw.ehu.eus/file.php/83/cap31_html/capitulo-3.html

carakenio73. "Dinámica de un sistema masa-resorte-amortiguador." dademuchconnection, 18 de julio de 2017, https://dademuchconnection.wordpress.com/2017/07/18/dinamica-de-un-sistema-masa-resorte-amortiguador/.

 

 

