# automatizacion-de-Pruebas
Curso para aprender que es y cuando conviene automatizar pruebas de software. Conocer los frameworks y herramientas mas utilizados

Ventajas y desventajas de la automatizacion 

# Ventajas
* Mejorar la eficiencia de las pruebas.
* Proporcionar una cobertura de pruebas mas amplia con respecto a las pruebas manuales
* Reducir el costo total de las pruebas, es decir, no implicar costos que generarian acciones innecesarias como las pruebas manuales
* Aumentar la frecuencia de las pruebas reduciendo el tiempo requerido para los ciclos de prueba.
* Se pueden ejecutar mas pruebas por compilacion o por liberacion
* La posibilidad de crear pruebas que no se pueden realizar manualmente, como las pruebas en tiempo real o pruebas paralelas.
* Las pruebas estan menos sujetas a errores del operador. Una ez que se haya programado no van a fallar.

# Desventajas
* Costos adicionales en herramientas, soluciones o profesionales,
* Requiere de conocimientos de programacion, lo que implica que sea mas dificil de solucionar errores o debuggear.
* Requiere un mantenimiento continuo porque el sofware evoluciona rapidamente. 
* Es necesario agragar tecnologias adicionales en el stack de tu empresa.
* Las pruebas pueden volverse complejas
* Distraccion de los objetivos de la prueba, a veces no se evalua correctamente los que se debe automatizar o lo que no
* Tiempos innecesarios en automatizar pruebas que hubieran sido resueltas mas rapido de forma manual


# Limitantes de la automatizacion de pruebas
Two factor authentication 
reCAPTCHA
Gmail
Sensores en dispositivos 
Solo se puede medir informacion que entiende la maquina
No va a remplazar a las pruebas exploratorias 
UX la experiencia del usuario 

# Tipos de pruebas
* Funcionales 
    Nos permiten analizar los requisito comerciales (lo que el cliente va a ver)
* No funcionales
    Nos permiten probar las cosas que son necesarias para que el cliente vea y tenga una experiencia agradable. (Rendimiento, seguridad, almacenamiento de datos etc)

Pruebas unitarias: Pequeños bloques de software que puedes ir automatizando y probando una funcionalidad pequeña y concreta; son las mas baratas y las hacen los mismos desarrolladores
Pruebas de integracion: Nos permite probar bloques en conjunto.
Pruebas de humo: Son pruebas que se corren despues de una liberacion o compilacion para asegurar que nada se haya incendiado y que todo funciona correctamente
Pruebas de regresion: Nos va a servir para garantizar que todo sigue funcionando correctamente cuando incluimos nuevas funcionalidades. 
Pruebas de APIs: puedes automatizar pruebas a los endPoints de una API para garantizar que funciona como debe
Pruebas de seguridad: Su proposito es identificar las vulnerabilidades de seguridad de un sistema (tambien conocidas como pruebas de Pentesting)
Pruebas de rendimiento: Son un tipo de pruebas no funcionales, porque nos permiten evaluar la estabilidad y aseguran que el sofware funcione adecuadamente.
Pruebas de aceptacion: Intentan determinar cual es el resultado esperado del cliente
Pruebas de UI: Son las pruebas de interfaz y nos permiten garantizar que el proyecto interactue como deberia. Se pueden hacer por bloques, por funcionalidad o pruebas end-to-end

SON TRES GRUPOS
Pruebas unitarias(desarrollador)
Pruebas de API (desarrollador backend, test automation o QA)
Pruebas de UI (pruebas end-to-end)

# Tipos de frameworks de automatizacion
* Capture/Playback: reproduce lo que hayas hecho durante una prueba
    Pros: El enfoque de captura/reproduccion se puede utilizar para el SUT (System under test) en el nivel de GUI/API. Inicialmente, es facil de configurar y usar. 
    Contras: Es dificil de mantener, por los cambios frecuentes, La implementacion de los casos de prueba (scripts) solo pueden comenzar hasta que el sistema esta disponible.
* Linear Scripting: Es parecido al anterior, pero este te produce un codigo el cual puedes cambiar y comentar,
    Pros: Se puede utilizar para probar el sistema a nivel GUI y/o API, facil de configurar
    Contras: cantidad de esfuerzo. Dificil de mantener. Costo de mantenimiento es lineal.
* Structured Scripting: Lo mismo pero reutilizando los scipst
    Pros: Reduccion de mantenimiento, reutilizacion de secuencias de comandos, costos de construccion y mantenimiento
    Contras: Esfuerzo inicial, Habilidades de programacion, Administracion
* Module based: Basado en POO, cambiios pueden ser por secciones
    Pros: Modular, escalable y flexible (facil mantenimiento)
    Contras: Sin flexibilidad en datos
* Data Driven: Tenemos mas entradas de prueba de base de datos(no harcoded)
    Pros: Costo, mayor cobertura, flexibilidad en ejecucion.
    Contras: Mas fuentes de datos, dominio de un lenguaje de programacion,
* keyword Driven: lo mismo que el diven, pero con  descripcion, como se llama el boton y donde esta localizado
    Pros: Flexibilidad en la creacion de pruebas, reutilizacion de codigo, No se requiere conocimiento de las secuencias de comando
    Contras: Complejidad de aprendizaje, Incremento de dificultad a medida que se introducen palabras clave
* Hybrid: convinacion entre data driven y keyword, le envia que datos requieren ese test
* Behavior Driven Development: Impulsado por el comportamiento, usa palabras reservadas en un lenguaje llamado gherkin (given, when, then)
    Pros: Mayor compatibilidad entre historias de usuario y test cases. Claridad en los casos de prueba. Reutilizacion de codigo. Data-driven
    Contras: Inversion de tiempo. Tiempo de planificacion. Conocimiento de Gherking o similar

