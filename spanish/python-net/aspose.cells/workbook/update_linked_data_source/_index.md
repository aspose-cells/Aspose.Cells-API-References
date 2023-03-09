---
title: update_linked_data_source método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 410
url: /es/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Si este libro de trabajo contiene enlaces externos a otra fuente de datos,
Aspose.Cells intentará recuperar los datos más recientes.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| external_workbooks | list | Este libro hace referencia a los libros de trabajo externos.<br/>Si es nulo, abriremos directamente los archivos vinculados externos.<br/>Si no es nulo,<br/>comprobaremos si el enlace externo en la matriz primero;<br/> si no, volveremos a abrir los archivos vinculados externos.|
###  Observaciones

Si no se llama al método antes de calcular fórmulas,
Aspose.Cells utilizará la información anterior (almacenada en caché en el archivo);
 Configure CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath.
Y configure Workbook.FilePath si este libro de trabajo es de una secuencia,
de lo contrario, Aspose.Cells a veces no podía obtener la ruta completa del enlace externo.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
