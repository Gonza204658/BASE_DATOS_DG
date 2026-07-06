# Análisis del archivo Excel

Cuando revisé el archivo de Excel vi que toda la información estaba mezclada en una sola tabla. Había datos de ciudades, proveedores, categorías, productos, compras y movimientos de inventario, lo que hacía que muchos datos se repitieran varias veces. También encontré nombres escritos de diferentes formas, aunque se referían a lo mismo, todo estaba desorganizado.



## Estructura inicial

Al principio toda la información estaba en un solo archivo, por lo que cada vez que aparecía un producto también se repetían el proveedor, la ciudad, la categoría y otros datos.



## Problemas identificados

Los principales problemas que encontré fueron:

* Información repetida.
* Nombres escritos de diferentes maneras, por ejemplo una misma ciudad o proveedor.
* Datos mezclados en una sola tabla.
* Mucha redundancia, ya que la misma información aparecía varias veces.


## Primera Forma Normal 

Primero me aseguré de que cada columna tuviera un solo dato y que cada registro representara una sola información. También definí un identificador único para cada tabla mediante una llave primaria.


## Segunda Forma Normal 

Después separé la información en varias tablas según su función, creé tablas para ciudades, proveedores, categorías, productos, almacenes, compras, detalles de compra y movimientos de inventario de esta forma cada tabla guarda únicamente la información que le corresponde

## Tercera Forma Normal 

Por último relacioné todas las tablas mediante llaves foráneas para evitar repetir información. Así, por ejemplo, un proveedor solo guarda el id de la ciudad y un producto solo guarda el id de su categoría. Esto hace que la base de datos sea mucho más organizada y fácil de mantener.

## Resultado final

Al finalizar el proceso obtuve una base de datos compuesta por ocho tablas relacionadas entre sí mediante llaves primarias y foráneas. Con este modelo eliminé la mayor parte de la información repetida del archivo original y logré una estructura organizada que cumple con la Primera, Segunda y Tercera Forma Normal.
