---
title: get_precedents metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Hämtar alla referenser som visas i den här cellens formel.


###  Returnerar

Samling av alla referenser som förekommer i denna cells formel.


```python
def get_precedents(self):
    ...
```


###  Anmärkningar

* Returnerar null om detta inte är en formelcell. Alla referenser som visas i den här cellens formel kommer att returneras oavsett om de refereras till eller inte under beräkningen.

Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
det tas fortfarande som formelns prejudikat. För att få de referenser som endast påverkar beräkningen, använd [Cell.get_precedents_in_calculation()](/cells/sv/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Returnerar null om detta inte är en formelcell. Alla referenser som visas i den här cellens formel kommer att returneras oavsett om de refereras till eller inte under beräkningen.
Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
det tas fortfarande som formelns prejudikat. För att få de referenser som endast påverkar beräkningen, använd [Cell.get_precedents_in_calculation()](/cells/sv/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Returnerar null om detta inte är en formelcell. Alla referenser som visas i den här cellens formel kommer att returneras oavsett om de refereras till eller inte under beräkningen.
Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
det tas fortfarande som formelns prejudikat. För att få de referenser som endast påverkar beräkningen, använd [Cell.get_precedents_in_calculation()](/cells/sv/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  Exempel

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



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
