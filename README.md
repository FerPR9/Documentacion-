# Documentacion

# Sistema de Gestión de Gimnasio - Sportacus Gym - Módulo CheckIn

# Integrantes 

* Marisol Nuñes Monasterio 
* Maria Fernanda Palacios Rangel 

# Descripsión 

El proyecto se enfoca en crear un sistema de gestión para el gimnasio Sportacus Gym, el cual consiste en varios módulos. Uno de los módulos más importantes es el de CheckIn, el cual permite que los empleados registren su hora de entrada y salida cada día al escanear un código QR. Esta funcionalidad también permite llevar un control de asistencias y retardos por cada empleado.
El módulo de CheckIn tiene tres funcionalidades principales. La primera es la generación de un código QR dinámico para cada empleado utilizando la API GoQR. La segunda es la posibilidad de registrar la entrada y salida de un empleado en la base de datos mediante la lectura del código QR. La tercera funcionalidad permite consultar los registros de asistencia de un empleado, donde se muestran los registros de entrada y salida, se tiene un calendario para visualizar las asistencias y retardos y se genera una gráfica con un resumen de las asistencias y retardos.
Este sistema permitirá mejorar la eficiencia de las operaciones en el gimnasio y el módulo de CheckIn permitirá a los administradores tener un control más ágil de las asistencias y retardos, manteniendo los registros actualizados.

# Objetivo general 

Implementar un sistema de control de asistencias mediante la generación y escaneo de códigos QR para los empleados del gimnasio, con el fin de registrar de manera eficiente y precisa las entradas, salidas, retardos y faltas de cada empleado. Además, utilizar esta información para incentivar la puntualidad y el compromiso de los empleados y tomar medidas disciplinarias en caso de faltas o retardos recurrentes, con el objetivo de mejorar la eficiencia y productividad del gimnasio.


# Objetivos especificos 

* Objetivos Específicos
* Registrar entrada y salida de los empleados del gimnasio.
* Controlar la asistencia y puntualidad de los empleados.
* Facilitar el cálculo de las asistencias y retardos de los empleados.
* Generar información estadística sobre la asistencia y puntualidad de los empleados.

# Propuesta de solucion

![image](https://user-images.githubusercontent.com/126131443/233436758-1a76bd6a-932a-4a1e-abcb-977325b4a86d.png)

# Diagra de actividad 

Registar asistencia 

![image](https://user-images.githubusercontent.com/126131443/233437072-5e4f456e-7239-48fc-850f-4c79a025f6e7.png)

Adminsitrar asitencia 

![image](https://user-images.githubusercontent.com/126131443/233437147-a65530b9-29bb-413a-9279-cef02965d18a.png)

# Historias de usuario

![image](https://user-images.githubusercontent.com/126131443/233437470-9952145a-14dc-4202-87be-6008f4cdd87e.png)

Administrar asisitencia 

![image](https://user-images.githubusercontent.com/126131443/233437564-17bfd063-4e48-4756-a868-0555f9fe3b23.png)


# Modelo vista controlador 
![image](https://user-images.githubusercontent.com/126131443/233433265-8110f9a5-854c-420b-b611-1e959d9b800e.png)

# Diagrama de componentes 
![Diagrma de componentes](https://user-images.githubusercontent.com/126131443/233441275-751a5d50-a587-4dd0-b39f-a01541d070b0.jpeg)

# Modelo de datos 

Check-In
![image](https://user-images.githubusercontent.com/126131443/233442200-061d5143-9d9e-4238-a5f3-18432cfeaaf8.png)

Empleado
![image](https://user-images.githubusercontent.com/126131443/233442300-1f37df09-c050-4547-bb01-d24a1f1a0971.png)


La colección de “Empleado” almacenara la información de los empleados registrados en los siguientes campos: 
*	IdEmpleado: es el id de identificador del empelado.
*	Nombre: Nombre del empelado del gimnasio. 
*	Edad: La edad del empleado del gimnasio.
*	Rol: Rol o actividad que desempeña el empleado dentro gimnasio (puede tener más de un rol).
*	Teléfono: Teléfono de contacto del empleado del gimnasio (puede tener más de un teléfono).
*	Sueldo: Cantidad de dinero que se le paga al empleado. 
*	Turno: Horario de trabajo del empleado (Matutino, Vespertino).
*	Correo: Dirección de correo electrónico de contacto del empleado. 
*	Password: Contraseña de usuario.


La colección de “Rol” almacena información de los roles asignados y desempeñados por los empleados: 

*	Nombre: Nombre del empleado que desempeña la actividad en el gimnasio. 
*	Descripción: Descripción de las actividades que desempeña la persona con el rol asignado. 
*	Privilegios: Privilegios asignados a partir de los roles, es decir las actividades que puede realizar en el sistema según su rol. 

La colección “Check-In” almacena información de los registros de asistencia de los empleados del gimnasio. 

*	IdEmpleado: Identificados o clave única de cada empleado del gimnasio. 
*	Fecha: Día, mes y año en que se realizan los registros de asistencia de los empelados del gimnasio. 
*	Hora: Hora de entrada y salida en que se realiza el registro en el check- in por medio del escaneo del Qr. 
*	Tipo: Hora de entrada o salida de registro de asistencia. 


# Estandares 



