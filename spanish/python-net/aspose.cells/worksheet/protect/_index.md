---
title: protect método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 180
url: /es/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Protege la hoja de trabajo.



```python
def protect(self, type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| type | [ProtectionType](/cells/es/python-net/aspose.cells/protectiontype) | Tipo de protección.|
###  Observaciones

Este método protege la hoja de trabajo sin contraseña. Puede protect hoja de trabajo en todas las versiones del archivo de Excel.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Protege la hoja de trabajo.



```python
def protect(self, type, password, old_password):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| type | [ProtectionType](/cells/es/python-net/aspose.cells/protectiontype) | Tipo de protección.|
| password | str | Contraseña.|
| old_password | str | Si la hoja de trabajo ya está protegida por una contraseña, proporcione la contraseña anterior.<br/> De lo contrario, puede establecer un valor nulo o una cadena en blanco para este parámetro.|
###  Observaciones

Este método puede protect hoja de trabajo en todas las versiones del archivo de Excel.
###  Ejemplo


```python
from aspose.cells import ProtectionType, Workbook

# Instantiating a Workbook object
excel = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = excel.worksheets[0]
# Protecting the worksheet with a password
worksheet.protect(ProtectionType.ALL, "aspose", None)
# Saving the modified Excel file in default (that is Excel 20003) format
excel.save("output.xls")

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Worksheet](/cells/es/python-net/aspose.cells/worksheet)
