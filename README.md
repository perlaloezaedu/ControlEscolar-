#ControlEscolar
# Incremento 1 — EduControl
# 1. Objetivo
Implementar la estructura inicial de clases, interfaces y la primera funcionalidad prioritaria, conectando la aplicación con la persistencia MySQL.

# 2. Arquitectura implementada
Se mantiene la arquitectura por capas definida en Sprint 2: Presentation/Controller, Service, DAO/Persistencia, Model y Config/Util.

# 3. Clases implementadas
Las siete entidades del modelo están representadas en `model`: Usuario, Alumno, Curso, ContenidoCurso, Inscripcion, Pago y Calificacion.

# 4. Interfaces
Se implementa `UsuarioDAO`, que define las operaciones de inserción y consulta. `UsuarioDAOImpl` contiene la implementación JDBC.

# 5. Flujo funcional completo
1.	El usuario selecciona Registrar.
2.	Controller recibe correo y rol.
3.	Service valida los datos.
4.	DAO ejecuta INSERT mediante JDBC.
5.	MySQL almacena el registro.
6.	La opción Consultar ejecuta SELECT y muestra los registros.

# 6. Persistencia
La conexión se centraliza en `Conexion.java`. Las consultas SQL se encuentran en la capa DAO.

# 7. Validaciones
·	Correo obligatorio.
·	Correo con formato básico válido.
·	Rol obligatorio.
·	Estado ACTIVO por defecto.
·	La base de datos conserva la restricción UNIQUE para `usuarios.correo` definida en Sprint 2.


##Integrantes:



