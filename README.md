# Diagrama-de-clases
Es un diagrama de un ejercicio Propuesto por Maximo
## Este es el enunciado del ejercicio

Una empresa de ventas online quiere que he hagas un diagrama de clases para organizar sus sistemas estos quieren saber los clientes; su código dirección, correo, nombre y apellidos estos últimos mediante una relación entre persona y clientes  Persona; queremos saber su ID, Nombre y Apellido también una persona puede ser cliente o vendedor, Vendedor; Queremos saber su nivel de acceso y que persona son También queremos saber qué productos vende Productos; queremos saber su Nombre, Precio, y su vendedor también queremos saber su nota De la nota queremos saber qué opinaba el cliente la nota en si el cliente que la puso y el nombre del producto Por último los clientes tendrán un carro donde se situarán todos los productos que quieren el cliente que los quiere y el nombre del carro.
Atributos:
Persona :
ID:El número que sirve como clave primaria para identificar la persona
Nombre: Es el nombre de dicha persona
Apellido: Son los apellidos de dichas personas
Cliente:
	CustomerID:El número que sirve como clave primaria para identificar la persona
	billingAddress:Es donde se envían los pedidos del cliente
	Email:Es el contacto del cliente para poder notificarte del envío
	Relaciones:
		PerID:Es la persona a la que se asocia esta cuenta
Vendedor:
	VendID:El número que sirve como clave primaria para identificar la persona
	AccesLevel:Es la importancia de dicho vendedor
	Relaciones:
		PerID:Es la persona a la que se asocia esta cuenta
Producto:
	Nombre:Es el nombre de dicho producto y su clave primaria ya que no hay dos con 
el mismo nombre
Precio:Es el costo del producto
Relaciones:
VenID:Es el vendedor que distribuye dicho producto
Nota:
	Texto:Es la información que da el cliente sobre la nota
	Nota: Es la puntuación numérica del producto
	Relaciones:
		Nombre:Es el nombre del producto y actúa como clave primaria junto con 		CustomerID:Es el cliente que ha escrito la reseña del producto
Carro:
	Nombre:Es el nombre del carro y actúa como clave primaria ya que se le asigna un 	valor aleatorio
	Relaciones:
		CustomerID:Es el nombre del cliente
		Nombre:Es el producto que está en el carro
