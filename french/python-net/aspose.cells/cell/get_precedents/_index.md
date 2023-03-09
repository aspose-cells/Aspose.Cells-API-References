---
title: get_precedents méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Obtient toutes les références apparaissant dans la formule de cette cellule.


###  Retour

Collection de toutes les références apparaissant dans la formule de cette cellule.


```python
def get_precedents(self):
    ...
```


###  Remarques

* Renvoie null s'il ne s'agit pas d'une cellule de formule. Toutes les références apparaissant dans la formule de cette cellule seront renvoyées, qu'elles soient référencées ou non lors du calcul.

Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
il est toujours considéré comme les précédents de la formule. Pour obtenir les références qui influencent uniquement le calcul, veuillez utiliser [Cell.get_precedents_in_calculation()](/cells/fr/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Renvoie null s'il ne s'agit pas d'une cellule de formule. Toutes les références apparaissant dans la formule de cette cellule seront renvoyées, qu'elles soient référencées ou non lors du calcul.
Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
il est toujours considéré comme les précédents de la formule. Pour obtenir les références qui influencent uniquement le calcul, veuillez utiliser [Cell.get_precedents_in_calculation()](/cells/fr/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Renvoie null s'il ne s'agit pas d'une cellule de formule. Toutes les références apparaissant dans la formule de cette cellule seront renvoyées, qu'elles soient référencées ou non lors du calcul.
Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
il est toujours considéré comme les précédents de la formule. Pour obtenir les références qui influencent uniquement le calcul, veuillez utiliser [Cell.get_precedents_in_calculation()](/cells/fr/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  Exemple

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



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
