Tablas y Estructura
1.	Empleado
o	EmpleadoID (PK): int
o	Nombre: varchar
o	Telefono: varchar
o	Tipo: varchar (puede ser "Cliente" o "Veterinario")
2.	Cliente (hereda de Empleado)
o	ClienteID (PK, FK): int (refiere a EmpleadoID)
o	Direccion: varchar
3.	Mascota (hereda de Empleado)
o	MascotaID (PK): int
o	Nombre: varchar
o	Especie: varchar
o	Edad: int
o	PropietarioID (FK): int (refiere a ClienteID)
4.	Factura
o	FacturaID (PK): int
o	Numero: int
o	Fecha: date
o	Total: float
o	ClienteID (FK): int (refiere a ClienteID)
o	MascotaID (FK): int (refiere a MascotaID)


