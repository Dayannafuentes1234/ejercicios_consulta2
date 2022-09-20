# ejercicios_consulta2

![tabla empleados](/img/tabla%20empleados.png "tabla empleados")

![tabla empleados](/img/tabla%20empleados1.0.png "tabla empleados1.0")

1. Traer el nombre, cedula y salario de un empleado, ordenando los campos de la siguiente manera: Ascendentey Descendente por cedula.

`SELECT nombre, cedula, sueldo FROM Empleados WHERE(ciudad ="medellin") ORDER BY nombre`

![consulta1](/img/consulta1.png "conuslta.1")

`SELECT nombre, cedula, sueldo FROM Empleados WHERE(ciudad ="medellin") ORDER BY cedula DESC`

![consulta1.0](/img/consulta1%2C0.png "conuslta.1.0")

2. Traer el nombre y salario de los primeros 10 empleados cuyo saldo es mayor a $600000 ordenandolos en forma ascendente por el numero de cedula.

`SELECT TOP 10 nombre, sueldo FROM empleado WHERE (sueldo>600000)ORDER BY cedula`

![consulta2](/img/consulta2.png "conuslta2")

3. Mostrar el nombre, id y cedula de los primero 15 empleados cuyos nombres sean distintos. Ordene la consulta en forma descendente por cedula.

`SELECT DISTINCT TOP 15 nombre, id, cedula FROM Empleado ORDER BY cedula DESC`

![consulta3](/img/consulta3.png "conuslta3")

4. Entregar los primeros 10 empleados con nombre y cedula cuya ciudad sea bogota. Se necesita que los encabezados de las columnas tengan los siguientes titulos:

a. para el campo nombre ------- Razon social
B. para el campo cedula ------- Identificacion
c. ordene la cedula en dorma descendente por cedula

`SELECT TOP 10 nombre AS "Razon social", cedula AS "Identificacion" FROM Empleado WHERE (ciudad="bogota")ORDER BY cedula DESC`

![consulta4](/img/consulta4.png"conuslta4")

5. Realizar una consulta que entregue el nombre, identificacion, sueldo, edad de los empleados cuyos sueldos estren entre $800000 y $1200000 y cuyas edades esten entre 23 y 30 años.

`SELECT nombre, cedula, sueldo, edad FROM empleado WHERE(sueldo BETWEEN 800000 AND 1200000 AND edad BETWEEN 23 AND 30)`

![consulta5](/img/consulta5.png "conuslta5")

6. Realizar una consulta que muestre nombre, cedula y salario de los empleados cuyo nombre comience con la letra c. Ordene esta lista por salario en forma descendente.

`SELECT nombre, cedula, sueldo FROM Empleado WHERE(nombre LIKE 'c%')ORDER BY sueldo DESC`

![consulta6](/img/consulta6.png "conuslta6")

