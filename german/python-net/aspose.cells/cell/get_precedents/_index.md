---
title: get_precedents Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Ruft alle Verweise ab, die in der Formel dieser Zelle vorkommen.


###  Kehrt zurück

Sammlung aller Referenzen, die in der Formel dieser Zelle vorkommen.


```python
def get_precedents(self):
    ...
```


###  Bemerkungen

* Gibt null zurück, wenn es sich nicht um eine Formelzelle handelt. Alle Referenzen, die in der Formel dieser Zelle erscheinen, werden zurückgegeben, unabhängig davon, ob sie während der Berechnung referenziert werden oder nicht.

Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Es wird immer noch als Präzedenzfall der Formel angesehen. Um die Referenzen zu erhalten, die nur die Berechnung beeinflussen, verwenden Sie bitte [Cell.get_precedents_in_calculation()](/cells/de/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Gibt null zurück, wenn es sich nicht um eine Formelzelle handelt. Alle Referenzen, die in der Formel dieser Zelle erscheinen, werden zurückgegeben, unabhängig davon, ob sie während der Berechnung referenziert werden oder nicht.
Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Es wird immer noch als Präzedenzfall der Formel angesehen. Um die Referenzen zu erhalten, die nur die Berechnung beeinflussen, verwenden Sie bitte [Cell.get_precedents_in_calculation()](/cells/de/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Gibt null zurück, wenn es sich nicht um eine Formelzelle handelt. Alle Referenzen, die in der Formel dieser Zelle erscheinen, werden zurückgegeben, unabhängig davon, ob sie während der Berechnung referenziert werden oder nicht.
Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Es wird immer noch als Präzedenzfall der Formel angesehen. Um die Referenzen zu erhalten, die nur die Berechnung beeinflussen, verwenden Sie bitte [Cell.get_precedents_in_calculation()](/cells/de/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  Beispiel

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



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
