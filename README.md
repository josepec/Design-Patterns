# Design-Patterns
 

## Creational (Creacionales) 

### Factory Method 

<p align="center">
  <img src="[your_relative_path_here](https://github.com/josepec/Design-Patterns/blob/master/img/1.png)" width="350">
</p>

Define una interfaz de creación de un tipo de objeto y permite a las subclases del mismo decidir que tipo de instancia concreta necesita. Se utiliza cuando necesitamos crear la instancia de un objeto que a priori no sabemos que tipo va a ser. 

Si deseamos crear un nuevo ‘ConcreteProduct’ se puede añadir al ‘Creator’ sin que afecte a la funcionalidad de la aplicación. Estando bastante desacoplado. No se necesitan clases específicas. 

 

### Abstract Factory 

  

Una fábrica de fábricas, del patrón ‘Factory Method’. Indicamos la fábrica del objeto que será la que lo cree. 

Oculta las clases de impletación. Los clientes pueden manipular los objetos a través de las interfaces o clases abstractas. Facilita el intercambio de la familia de objetos y promueve la consistencia entre los objetos.  

 

### Builder 

 

Nos permite crear objetos complejos a partir de un objeto fuente (Producto). Objetos compuestos por muchos atributos. Se independiza de las partes que lo componen y del ensamblado. 

Reduce el acoplamiento. Permite crear estructuras complejas respetando la interfaz común de la clase builder. El código de construcción es independiente del de representación. Da un mayor control en el proceso de creación de objetos. 

 

### Prototype 

 

Crea objetos a partir de un modelo. Especificar el tipo de objetos que se crearán mediante una instancia prototípica y crear nuevos objetos copiando ese prototipo. Permite que un objeto cree una copia de si mismo (clonar) sin conocer su clase ni ningún detalle. 

Clonar un objeto siempre es más rápido que crearlo. Es bueno usarlo cuando la creación de los objetos es muy pesada. Aparte, oculta la complejidad de un objeto y podemos agregar y quitar cualquier objeto en tiempo de ejecución. 

 

### Singleton 

 

Permite que el mismo objeto sea siempre compartido en distintas partes del código.  Haciendo que la clase tenga únicamente una instancia y haya un punto de acceso global a ella. 

Proporciona un acceso controlado a la única instancia de la clase. Por ejemplo para base de datos. 

 

## Behavioral (Comportamiento) 

### Chain of Responsability 

 

Permite que varias clases intenten manejar una solicitud. Ideal cuando una solicitud por parte de un objeto  debe de ser atendida por parte de distintos objetos receptores sin saber qué objeto puede resolver el problema. Se intenta resolver la solicitud de manera jerárquica, si un objeto no sabe responder a la solicitud, se la pasa al siguiente. 

Reduce el grado de acoplamiento. No se necesita conocer la estructura de la cadena. Permite agregar o cambiar el orden de los miembros de la cadena. 

 

### Command 

 

Abstrae la lógica de negocio en acciones discretas de comandos. Encapsula la información para realizar acciones.  

Hace que nuestro código sea extendible, ya que nos permite añadir comandos fácilmente. 

 

### Iterator 

 

Nos ofrece un mecanismo estándar para acceder a los elementos de una colección. Proporciona una manera de acceder a los elementos sin exponer su estructura interna. 

 

### Mediator 

 

Permite el desacoplamiento de los objetos mediante una capa intermedia. Simplifica la comunicación entre los objetos (Tipo uno a muchos). 

 

### Memento 

 

Se utiliza para restaurar el estado de un objeto a un estado anterior.  

 

### Observer 

 

Implementa una estrategia que reacciona a los cambios de estado del objeto observado. Notifica a todos los observadores que ha cambiado. 

 

### State 

 

El objetivo es que un objeto modifique su comportamiento según su estado. 

Permite agregar fácilmente nuevos comportamientos y estados. Reduce el uso de sentencias if-else. 

 

### Interpreter 

 

Dado un lenguaje, define una representación para su gramática junto con un intérprete del lenguaje. Es fácil cambiar la gramática e introducir nuevas formas de interpretar la gramática. 

 

### Strategy 

 

Nos permite elegir una implementación específica de algoritmo o tarea en tiempo de ejecución. Encapsula los algoritmos en clases, y en tiempo de ejecución se elige el que ejecutamos. 

Se pueden ampliar los algoritmos de manera muy sencilla. 

 

### Template 

 

Define los pasos secuenciales para ejecutar un algoritmo de varios pasos. Define su estructura y la lógica se implementa en sus subclases. 

 

### Visitor 

 

Permite separar un algoritmo de la estructura del objeto en la que opera. Se pueden agregar nuevas operaciones a la estructura del objeto sin modificar la estructura. La clase ‘Visitor’ cambia el algoritmo de ejecución de una clase ‘Element’ y puede variar cuando el ‘Visitor’ varía. 

 

## Structural (Estructurales) 

### Adapter 

 

Hace que dos interfaces incompatibles, solucionen sus problemas entre sí. Es decir, que dos interfaces no interrelacionadas, trabajen entre sí. 

 

### Bridge 

 

Cuando tenemos que desacoplar una abstracción de su implementación, para que ambos puedan variar independientemente. 

Los cambios en la implementación de una abstracción no nos afectan al cliente. 

 

### Composite 

 

Nos permite construir objetos complejos o algoritmos, a partir de objetos o algoritmos más simples, gracias a la composición recursiva y a una estructura en forma de árbol. 

Se utilizan los objetos primitivos y compuestos de una manera uniforme, a través de una interfaz de componentes. 

 

### Decorator 

 

Se utiliza para agregar características o funcionalidades a una instancia particular de una clase sin llegar a modificar las demás instancias de la clase. Decorar un objeto, añade más responsabilidades a los objetos de manera dinámica. 

 

### Facade 

 

Simplifica el sistema para el cliente, proporcionando una interfaz unificada para un conjunto de subsistemas. Define una interfaz de alto nivel. 

Ocultamos la complejidad del subsistema para que lo utilice fácilmente. 

 

### Flyweight 

 

Permite el uso compartido de objetos para soportar grandes cantidades de objetos pequeños, de manera eficiente. Actúa como un objeto independiente en cada contexto. Útil con grandes cantidades de objetos, muy similares, que se diferencian en pocos atributos. 

Reduce el número de objetos en el sistema.  

 

### Proxy 

 

Se utiliza como intermediario, controlando el acceso. Que actúa como el objeto original, delegándole las llamadas. 
