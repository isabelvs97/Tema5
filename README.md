
# Laboratorio 5


De los datos del problema,se tiene que:

<img src="https://render.githubusercontent.com/render/math?math=\lambda = 2">. Para tener una fila de al menos un cliente el 90% del tiempo se necesita:

Utilizando las ecuaciones desarolladas anteriormente en el enunciado, se obtiene \nu:

<img src="https://render.githubusercontent.com/render/math?math=P( \text{1 o más clientes en el sistema} ) = \sum_{i=1}^{\infty} (1 - \rho) \rho^i  =1-\sum_{i=0}^{1} (1 - \rho) \rho^i = \rho^2">

<img src="https://render.githubusercontent.com/render/math?math=P( \text{1 o más clientes en el sistema} ) =\rho^2 & = \left( \frac{\lambda}{\nu} \right)^2 \geq 0.9"> 
<img src="https://render.githubusercontent.com/render/math?math=\nu^2 \geq \frac{\lambda^2}{0.9} = \frac{4}{0.9} = 4.44 \quad \Rightarrow \quad \nu \geq 2.11">

Se realizan modificaciones en el código a los valores:
  1. lam
  2. nu (v)/60
  3. P =1
  4. Condición para cumplir la especificación. La igualdad se cambia a fraccion>=0.10, que sería el 10% de tiempo mínimo que se debe estar atendiendo solicitudes. 
