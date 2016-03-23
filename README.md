# Scaffold 
(hay que elegir un nombre para el sistema)

## Requerimientos del Sistema
El Sistema con el cual se trabajo en el análisis se enfoca en la **gestión de una casa de compra y ventas de repuesto de automóviles** (siéntanse en libertad de elegir el nombre que más les guste).
La empresa **compra repuestos** de **diferentes procedencias** (china, Japón, Brasil, etc) por medio de sus **proveedores** (necesitamos guardar los datos del proveedor), generalmente de **contado** , pero eventualmente pueden librarse **cheques de 30, 60 y 90 días**, de los cuales solo debemos guardar los **datos del cheque** (fecha de emisión, cobro, nombre de orden, monto, etc). Una vez que **la factura es guardada en el sistema la reimpresión de la misma es opcional**.
Cada **repuesto pertenece a una categoría** , por ej.  Podríamos tener la categoría “Freno” y pastilla de freno es un repuesto que pertenece a esa categoría, como también disco de freno es otro repuesto de la categoría. Los **repuestos pueden pertenecer a un modelo de automóvil** (marca y modelo) particular, como así también **pueden ser genéricos**. Ej. Un bomba de inyección es particular de un automóvil (no le va a otro) en cambio un filtro de combustible puede ser genérico (funciona en varios modelos de automóviles).
La empresa posee **clientes**, de los cuales nos interesa saber **todos los datos del mismo** (puede ser una persona o una empresa).
La empresa **realiza presupuestos** y **facturas de ventas** (note que un presupuesto se convierte en factura simplemente al ser procesado en caja). Las **facturas pueden ser solo de contado** (no es necesario tomar el caso de venta a crédito) y las mismas **son procesadas en caja**. Es necesario **realizar la impresión de la factura generada** para ello asuma de que se realiza en un **formato pre-impreso**.
La empresa **posee un solo puesto de caja** de la cual se realiza **una apertura diaria indicando el monto de dinero con el que cuenta inicialmente** y **el cierre de la misma una vez finalizadas las transacciones del día** (el procesamiento de las facturas de venta y egresos que puedan haber). A la vez por **cada factura procesada en caja la misma genera un movimiento de caja** como **así también los egresos que puedan haber** (tener en cuenta para los informes, más abajo indicados).
De los egresos que pueden haber solo nos interesa saber el concepto y el monto del mismo. Es importante en todo momento saber **el saldo actual de caja (ingresos - egresos)**.
El sistema **no necesita de roles**, pero indispensablemente se debe **registrar al usuario en el sistema** para que el mismo pueda loguearse mostrando en la pantalla principal sus datos.

## Informes
- Resumen de ventas por periodos: informe en el cual se presenta de manera tabular la fecha de la venta,  el numero de factura, el cliente y el monto en el periodo de tiempo seleccionado.
###### Ejemplo

                                              **RESUMEN DE VENTAS**
                                 DESDE: 21/12/2016               HASTA:23/12/2016

                  | Fecha        | Num. Factura | Cliente                       | Monto      | 
                  |:------------:|:------------:|:-----------------------------:|:----------:|
                  | 21/12/2016   | 12345        | Jorge García                  | 150.000    |
                  | 21/12/2016   | 12346        | Juan Francisco da Vinci Perez | 1.500.000  |
                  | 22/12/2016   | 12347        | Manuel Sanchez                | 850.000    |
                  | 22/12/2016   | 12348        | Autorepuestos Parana          | 5.405.400  |
                  | 23/12/2016   | 12349        | Autorepuestos Brasil          | 5.000.000  |
                  | 23/12/2016   | 12350        | Algun Otro                    | 15.000.000 |
                  | Total en Guaraníes                                          | 26.255.400 |

- Listado de movimientos de caja por día (similar al informe superior, detallando ingreso o egreso y el total de la caja).
- Resumen de cajas por periodos, indicando la fecha y el saldo con el que se cerró la caja ese día (presentando al final del informe la sumatoria de los saldos del periodo indicado).

## Entregas

##### Primera Entrega **17 de Abril**
- Menu: es necesario que ya esten todos los elementos, aquellos items que ya tienen implementado ya tienene que apuntar
- ABMs
  * Proveedores
  * Categorías
  * Repuestos
  * Marcas
  * Clientes
  * Modelos
  * Usuarios

##### Segunda Entrega **.. de Mayo**
- Modelado de bd general
- Login
- Cheque
- Factura
- Presupuesto

##### Tercera entrega **.. de Junio**
- Caja
- Movimientos de caja
- Arqueo de caja
- Reportes

