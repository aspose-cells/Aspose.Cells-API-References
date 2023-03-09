---
title: register_add_in_function método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 170
url: /es/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Agrega la función addin al libro de trabajo


###  Devoluciones

URL del archivo de complemento que contiene funciones de complemento


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| id | int | ID de los datos que contienen funciones adicionales,<br/> se puede obtener con la primera llamada al [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/es/python-net/aspose.cells/worksheetcollection/register_add_in_function) para el mismo archivo de complemento.|
| function_name | str | el nombre de la función de adición|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Agrega la función addin al libro de trabajo


###  Devoluciones

ID de los datos que contienen la función de complemento dada


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| add_in_file | str | el archivo contiene las funciones adicionales|
| function_name | str | el nombre de la función de adición|
| lib | bool | si el archivo de complemento dado está en el directorio o subdirectorio de la biblioteca de complementos del libro de trabajo.<br/>Esta bandera surte efecto y marca la diferencia cuando addInFile tiene una ruta relativa:<br/> true indica que la ruta es relativa a la biblioteca de complementos y false indica que la ruta es relativa a este libro de trabajo.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [WorksheetCollection](/cells/es/python-net/aspose.cells/worksheetcollection)
