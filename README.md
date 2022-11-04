# Design-Patterns
 

## Creational (Creacionales) 

### Factory Method 

 ![](https://github.com/josepec/Design-Patterns/blob/master/img/1.png)

Define una interfaz de creación de un tipo de objeto y permite a las subclases del mismo decidir que tipo de instancia concreta necesita. Se utiliza cuando necesitamos crear la instancia de un objeto que a priori no sabemos que tipo va a ser. 

Si deseamos crear un nuevo ‘ConcreteProduct’ se puede añadir al ‘Creator’ sin que afecte a la funcionalidad de la aplicación. Estando bastante desacoplado. No se necesitan clases específicas. 

 

### Abstract Factory 

   ![](https://github.com/josepec/Design-Patterns/blob/master/img/2.png)

Una fábrica de fábricas, del patrón ‘Factory Method’. Indicamos la fábrica del objeto que será la que lo cree. 

Oculta las clases de impletación. Los clientes pueden manipular los objetos a través de las interfaces o clases abstractas. Facilita el intercambio de la familia de objetos y promueve la consistencia entre los objetos.  

 

### Builder 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/3.png)

Nos permite crear objetos complejos a partir de un objeto fuente (Producto). Objetos compuestos por muchos atributos. Se independiza de las partes que lo componen y del ensamblado. 

Reduce el acoplamiento. Permite crear estructuras complejas respetando la interfaz común de la clase builder. El código de construcción es independiente del de representación. Da un mayor control en el proceso de creación de objetos. 

 

### Prototype 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/4.png)

Crea objetos a partir de un modelo. Especificar el tipo de objetos que se crearán mediante una instancia prototípica y crear nuevos objetos copiando ese prototipo. Permite que un objeto cree una copia de si mismo (clonar) sin conocer su clase ni ningún detalle. 

Clonar un objeto siempre es más rápido que crearlo. Es bueno usarlo cuando la creación de los objetos es muy pesada. Aparte, oculta la complejidad de un objeto y podemos agregar y quitar cualquier objeto en tiempo de ejecución. 

 

### Singleton 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/5.png)

Permite que el mismo objeto sea siempre compartido en distintas partes del código.  Haciendo que la clase tenga únicamente una instancia y haya un punto de acceso global a ella. 

Proporciona un acceso controlado a la única instancia de la clase. Por ejemplo para base de datos. 

 

## Behavioral (Comportamiento) 

### Chain of Responsability 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/6.png)

Permite que varias clases intenten manejar una solicitud. Ideal cuando una solicitud por parte de un objeto  debe de ser atendida por parte de distintos objetos receptores sin saber qué objeto puede resolver el problema. Se intenta resolver la solicitud de manera jerárquica, si un objeto no sabe responder a la solicitud, se la pasa al siguiente. 

Reduce el grado de acoplamiento. No se necesita conocer la estructura de la cadena. Permite agregar o cambiar el orden de los miembros de la cadena. 

 

### Command 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/7.png)

Abstrae la lógica de negocio en acciones discretas de comandos. Encapsula la información para realizar acciones.  

Hace que nuestro código sea extendible, ya que nos permite añadir comandos fácilmente. 

 

### Iterator 

 ![](https://github.com/josepec/Design-Patterns/blob/master/img/8.png) 

Nos ofrece un mecanismo estándar para acceder a los elementos de una colección. Proporciona una manera de acceder a los elementos sin exponer su estructura interna. 

 

### Mediator 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/9.png)

Permite el desacoplamiento de los objetos mediante una capa intermedia. Simplifica la comunicación entre los objetos (Tipo uno a muchos). 

 

### Memento 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/10.png)

Se utiliza para restaurar el estado de un objeto a un estado anterior.  

 

### Observer 

 ![](https://github.com/josepec/Design-Patterns/blob/master/img/11.png) 

Implementa una estrategia que reacciona a los cambios de estado del objeto observado. Notifica a todos los observadores que ha cambiado. 

 

### State 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/12.png)

El objetivo es que un objeto modifique su comportamiento según su estado. 

Permite agregar fácilmente nuevos comportamientos y estados. Reduce el uso de sentencias if-else. 

 

### Interpreter 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/13.png)

Dado un lenguaje, define una representación para su gramática junto con un intérprete del lenguaje. Es fácil cambiar la gramática e introducir nuevas formas de interpretar la gramática. 

 

### Strategy 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/14.png)

Nos permite elegir una implementación específica de algoritmo o tarea en tiempo de ejecución. Encapsula los algoritmos en clases, y en tiempo de ejecución se elige el que ejecutamos. 

Se pueden ampliar los algoritmos de manera muy sencilla. 

 

### Template 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/15.png)

Define los pasos secuenciales para ejecutar un algoritmo de varios pasos. Define su estructura y la lógica se implementa en sus subclases. 

 

### Visitor 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/16.png)

Permite separar un algoritmo de la estructura del objeto en la que opera. Se pueden agregar nuevas operaciones a la estructura del objeto sin modificar la estructura. La clase ‘Visitor’ cambia el algoritmo de ejecución de una clase ‘Element’ y puede variar cuando el ‘Visitor’ varía. 

 

## Structural (Estructurales) 

### Adapter 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/17.png)

Hace que dos interfaces incompatibles, solucionen sus problemas entre sí. Es decir, que dos interfaces no interrelacionadas, trabajen entre sí. 

 

### Bridge 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/18.png)

Cuando tenemos que desacoplar una abstracción de su implementación, para que ambos puedan variar independientemente. 

Los cambios en la implementación de una abstracción no nos afectan al cliente. 

 

### Composite 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/19.png)

Nos permite construir objetos complejos o algoritmos, a partir de objetos o algoritmos más simples, gracias a la composición recursiva y a una estructura en forma de árbol. 

Se utilizan los objetos primitivos y compuestos de una manera uniforme, a través de una interfaz de componentes. 

 

### Decorator 

 ![](https://github.com/josepec/Design-Patterns/blob/master/img/20.png) 

Se utiliza para agregar características o funcionalidades a una instancia particular de una clase sin llegar a modificar las demás instancias de la clase. Decorar un objeto, añade más responsabilidades a los objetos de manera dinámica. 

 

### Facade 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/21.png)

Simplifica el sistema para el cliente, proporcionando una interfaz unificada para un conjunto de subsistemas. Define una interfaz de alto nivel. 

Ocultamos la complejidad del subsistema para que lo utilice fácilmente. 

 

### Flyweight 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/22.png)

Permite el uso compartido de objetos para soportar grandes cantidades de objetos pequeños, de manera eficiente. Actúa como un objeto independiente en cada contexto. Útil con grandes cantidades de objetos, muy similares, que se diferencian en pocos atributos. 

Reduce el número de objetos en el sistema.  

 

### Proxy 

  ![](https://github.com/josepec/Design-Patterns/blob/master/img/23.png)

Se utiliza como intermediario, controlando el acceso. Que actúa como el objeto original, delegándole las llamadas. 
