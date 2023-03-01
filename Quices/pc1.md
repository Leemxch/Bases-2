# Prueba corta #1
## Max Richard Lee Chung - 2019185076
1. Explique como afectan los siguientes componentes el rendimiento de un sistema de base de datos:
* Disco: Los file system almacenan la información de las bases de datos, sin embargo, empeora mucho el rendimiento de la bases de datos por tener que ir a visitar hasta el disco para solicitar los datos.
* Memoria Virtual: Crea un espacio en disco pero más lento con una estructura similar pero diferente a un árbol binario para buscar los datos. 
* Memoria: Almacena el sistema operativo, por lo que debe de ser lo más rápido para acceder y manejar los datos. 
* Caché de CPU: Permite tener los datos precargados para aumentar el rendimiento del tiempo de respuesta sin tener que ir al disco, el cual aumenta el tiempo necesitado.
* CPU: Dependiendo de la cantidad de programas en ejecución, las aplicaciones (incluyendo la base de datos), compiten por el uso del hardware para procesar la información deseada, por lo que puede tener un buen rendimiento al tener pocas aplicaciones activas. El rendimiento puede empeorar si se dan muchos context switches porque se colapsa por el tránsito. 

2. ¿De que forma se benefician las aplicaciones del uso de caches? Explique.

Las aplicaciones se benefician por la localidad de los datos para poder acceder de forma inmediata a las páginas deseadas que se necesitan para el programa o alguna consulta de bases de datos. 

3. Desde el punto de vista de Elasticsearch, ¿Que es un índice?
 
Un índice son documentos que pueden ser buscados en casi tiempo real, el cual utiliza un método invertido de índices para realizar búsquedas de texto. Además, podría ser considerada como una colección optimizada, en donde cada campo y cada campo indexado tiene una estructura de datos dedicada y optimizada. Tiene la ventaja de ser schemeless o sin esquema/estructura para almacenar índices sin tener que definir cómo manejar los diferentes campos. 

4. ¿Que es un mapping en Elasticsearch?

El mapping o mappeo en Elasticsearch es dinámico, el cual permite agregar campos nuevos de forma automática para tener mayor facilidad a la hora de indexar y explorar la información. Dicho método se le pueden agregar condicionales para controlar cómo se quieren añadir la nueva información de entrada.  