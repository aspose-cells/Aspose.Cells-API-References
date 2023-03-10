---
title: check_excel_restriction propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction propiedad

Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas.
Por ejemplo, Excel no permite ingresar un valor de cadena de más de 32K.
Cuando ingresa un valor de más de 32 K, como Cell.PutValue (cadena), si esta propiedad es verdadera, obtendrá una excepción.
Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego
puede generar el valor de cadena completo para otros formatos de archivo como CSV.
Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel,
no debe guardar el libro de trabajo como formato de archivo de Excel más adelante. De lo contrario, puede haber un error inesperado para el archivo de Excel generado.
###  Definición:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [AbstractTextLoadOptions](/cells/es/python-net/aspose.cells/abstracttextloadoptions)
