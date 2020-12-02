
##Laboratorio 5


De los datos del problema,se tiene que:

<img src="https://render.githubusercontent.com/render/math?math=\lambda = 2">. Para tener una fila de al menos un cliente el 90% del tiempo se necesita:

Utilizando las ecuaciones desarolladas anteriormente en el enunciado, se obtiene \nu:

<img src="https://render.githubusercontent.com/render/math?math=P( \text{1 o más clientes en el sistema} ) = \sum_{i=1}^{\infty} (1 - \rho) \rho^i  = 1 - \sum_{i=0}^{0} (1 - \rho) \rho^i = 1-\rho">

<img src="https://render.githubusercontent.com/render/math?math=P( \text{1 o más clientes en el sistema} ) =1- \rho & = \left( \frac{\lambda}{\nu} \right)^1 \leq 0.1 \nu^1 & \geq \frac{\lambda^1}{0.1} = \frac{2}{0.1} = 20 \quad \Rightarrow \quad \nu \geq 20">

Se realizan modificaciones en el código a los valores:
  1. lam
  2. nu
  3. P (esto puede ser un valor elegido, ya que lo importante es tener solicitudes el 90% del tiempo)
  4. Frecuencia. Corresponde al tiempo con P o más solicitudes en sistema, lo cual equivale al 90% del tiempo. [0.90*len(t)]
  5. COndición para cumplir la especificación. La igualdad se cambia a fraccion>=0.10, que sería el 10% de tiempo mínimo que se debe estar atendiendo solicitudes. 
