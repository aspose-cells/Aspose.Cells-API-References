---
title: get_precedents método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 180
url: /es/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Obtiene todas las referencias que aparecen en la fórmula de esta celda.


###  Devoluciones

Colección de todas las referencias que aparecen en la fórmula de esta celda.


```python
def get_precedents(self):
    ...
```


###  Observaciones

* Devuelve nulo si esta no es una celda de fórmula Todas las referencias que aparecen en la fórmula de esta celda se devolverán sin importar si se hace referencia a ellas o no durante el cálculo.

Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
todavía se toma como los precedentes de la fórmula. Para obtener aquellas referencias que solo influyen en el cálculo, utilice [Cell.get_precedents_in_calculation()](/cells/es/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Devuelve nulo si esta no es una celda de fórmula Todas las referencias que aparecen en la fórmula de esta celda se devolverán sin importar si se hace referencia a ellas o no durante el cálculo.
Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
todavía se toma como los precedentes de la fórmula. Para obtener aquellas referencias que solo influyen en el cálculo, utilice [Cell.get_precedents_in_calculation()](/cells/es/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Devuelve nulo si esta no es una celda de fórmula Todas las referencias que aparecen en la fórmula de esta celda se devolverán sin importar si se hace referencia a ellas o no durante el cálculo.
Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
todavía se toma como los precedentes de la fórmula. Para obtener aquellas referencias que solo influyen en el cálculo, utilice [Cell.get_precedents_in_calculation()](/cells/es/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  Ejemplos

```python
from aspose.cells import CellsHelper, Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1"
areas = cells.get("A1").get_precedents()
for i in range(len(areas)):
    area = areas[i]
    stringBuilder = []
    if area.is_external_link:
        stringBuilder.append("[")
        stringBuilder.append(area.external_file_name)
        stringBuilder.append("]")
    stringBuilder.append(area.sheet_name)
    stringBuilder.append("!")
    stringBuilder.append(CellsHelper.cell_index_to_name(area.start_row, area.start_column))
    if area.is_area:
        stringBuilder.append(":")
        stringBuilder.append(CellsHelper.cell_index_to_name(area.end_row, area.end_column))
    print("".join(stringBuilder))

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
