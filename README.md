# biblioteca-parcial3
El programa está dividido en varias clases dentro de un mismo archivo, cada una con su función específica (principio de responsabilidad única, SRP).

BibliotecaApp.java
	Excepciones personalizadas
Se crean excepciones específicas para controlar errores esperados.
	Enum (EstadoPrestamo)
Define un tipo de dato enumerado con tres valores posibles.
	Clase Libro
Representa un libro dentro del sistema.
Se usan atributos encapsulados (private) para proteger los datos.
	Clase Usuario
Representa a un usuario registrado en la biblioteca.
Usa AtomicInteger para generar un ID único y seguro incluso en entornos concurrentes.
	Clase Prestamo
 Representa la relación entre un libro y un usuario (un préstamo activo o finalizado).
Guarda fechas de préstamo y devolución.
	Clase Biblioteca
Es el núcleo del sistema, donde se gestiona toda la información.
	Clase principal (BibliotecaApp) → Menú
 Proporciona una interfaz de consola para interactuar con el sistema.
 Muestra un menú con opciones.

 Lógica:
•	Usa Scanner para leer entradas del usuario.
•	Cada opción llama al método correspondiente de la clase Biblioteca.
•	Usa bloques try-catch para capturar excepciones personalizadas y mostrar mensajes claros.


Concepto:	Ejemplo en el código
POO (clases y objetos):     Libro, Usuario, Prestamo, Biblioteca
Encapsulación:          	Atributos private, métodos public controlados
Validaciones y reglas:  	ISBN, año, email, límites de préstamo
Excepciones personalizadas:   	LibroNoDisponibleException, UsuarioSinCupoException
Colecciones:  	HashMap, ArrayList, Streams
Concurrencia:  	synchronized, AtomicInteger
BigDecimal:   	Multas y cálculos monetarios
Streams y filtros:   	Reportes de top libros y usuarios con multa
Interfaz de consola:   	Menú interactivo con Scanner
Interfaz de consola	Menú interactivo con Scanner

