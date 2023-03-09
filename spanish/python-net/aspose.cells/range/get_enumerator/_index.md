---
title: get_enumerator método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 90
url: /es/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Obtiene el enumerador de las celdas de este rango.


###  Devoluciones

El enumerador de células


```python
def get_enumerator(self):
    ...
```


###  Observaciones

Al atravesar elementos por el Enumerador devuelto, la colección de celdas
no debe modificarse (como las operaciones que harán que se cree una nueva fila Cell o que se elimine la fila Cell existente).
De lo contrario, es posible que el enumerador no pueda recorrer todas las celdas correctamente (algunos elementos pueden recorrerse repetidamente u omitirse).
###  Ejemplo

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Range](/cells/es/python-net/aspose.cells/range)
