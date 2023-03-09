---
title: characters método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Devuelve un objeto Characters que representa un rango de characters dentro del texto de la celda.


###  Devoluciones

Objeto de los personajes.


```python
def characters(self, start_index, length):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| start_index | int | El índice del inicio del carácter.|
| length | int | El número de caracteres.|
###  Observaciones

Este método solo funciona en celdas con valor de cadena.
###  Ejemplo


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
