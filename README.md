# Sistema de Cálculo de Costo para Plantaciones Automatizadas

## Descripción
Este proyecto ayuda a determinar el costo de un sistema de plantaciones automatizado en Pythonia, luego de una grave sequía que afectó la región. Se basa en la división de un terreno en sembradíos cuadrados y el cálculo del costo total de sensores necesarios para la plantación, aplicando descuentos según el volumen de compra y subsidios gubernamentales.

## Funcionamiento
1. **Entrada de datos**:
   - Se solicita el **ancho** y **largo** del terreno (números enteros).
   - Se ingresa el **lado** de cada sembradío (número entero positivo).
   - Si el lado del sembradío es mayor que el ancho o el largo, el programa mostrará un error y finalizará.

2. **Cálculo de sembradíos**:
   - Se determina el número total de sembradíos en el terreno.

3. **Cálculo del costo de sensores**:
   - Cada metro cuadrado de sembradío requiere:
     - **4 sensores de humedad**
     - **1 sensor de temperatura**
     - **3 sensores de pH**
   - Los precios unitarios de los sensores dependen de la cantidad total de sembradíos según la siguiente tabla:

| n (cantidad de sembradíos) | Sensor humedad | Sensor temperatura | Sensor pH |
|----------------------------|---------------|---------------------|-----------|
| n <= 200                  | $350          | $450                | $1400     |
| 200 < n <= 400            | $300          | $350                | $1200     |
| 400 < n <= 1000           | $250          | $250                | $1000     |
| n > 1000                  | $200          | $150                | $800      |

4. **Aplicación de subsidios**:
   - El gobierno de Pythonia otorga un subsidio de **$15 millones** por cada **10.000 m2** efectivamente plantados.
   - Este subsidio se descuenta del monto total.

5. **Salida de resultados**:
   - Se muestra el costo final en **millones de dólares**, redondeado a **2 decimales**.

## Tecnologías Utilizadas
- Python
- Algoritmos de cálculo y optimización

## Contribuciones
Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, por favor abre un issue o envía un pull request.


