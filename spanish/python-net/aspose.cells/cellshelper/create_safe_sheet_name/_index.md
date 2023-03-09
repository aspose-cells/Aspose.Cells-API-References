---
title: create_safe_sheet_name método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 90
url: /es/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Comprueba el nombre de la hoja dada y crea uno válido cuando sea necesario.
Si el nombre de la hoja dado se ajusta a las reglas del nombre de la hoja de Excel, devuélvalo.
De lo contrario, la cadena se truncará si la longitud excede el límite
los caracteres no válidos se reemplazarán con ' ', luego devolverá el valor de la cadena reconstruida.


###  Devoluciones




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| name_proposal | str | nombre de la hoja a utilizar|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Comprueba el nombre de la hoja dada y crea uno válido cuando sea necesario.
Si el nombre de la hoja dado se ajusta a las reglas del nombre de la hoja de Excel, devuélvalo.
De lo contrario, la cadena se truncará si la longitud excede el límite
y los caracteres no válidos se reemplazarán con el carácter dado, luego devolverán el valor de la cadena reconstruida.


###  Devoluciones




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| name_proposal | str | nombre de la hoja a utilizar|
| replace_char | char | carácter que se utilizará para reemplazar los caracteres no válidos en el nombre de la hoja dada|



###  Ver también
* módulo [aspose.cells](../../)
* clase [CellsHelper](/cells/es/python-net/aspose.cells/cellshelper)
