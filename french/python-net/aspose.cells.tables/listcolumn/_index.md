---
title: ListColumn classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 10
url: /fr/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn classe
Représente une colonne dans une liste.



Le type ListColumn expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [name](/cells/fr/python-net/aspose.cells.tables/listcolumn/name) | Obtient et définit le nom de la colonne.|
| [totals_calculation](/cells/fr/python-net/aspose.cells.tables/listcolumn/totals_calculation) | Obtient et définit le type de calcul dans la ligne Totaux de la colonne de liste.|
| [range](/cells/fr/python-net/aspose.cells.tables/listcolumn/range) | Obtient la plage de cette colonne de liste.|
| [formula](/cells/fr/python-net/aspose.cells.tables/listcolumn/formula) | Obtient et définit la formule de la colonne de liste.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/fr/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | Obtient la formule de la ligne des totaux de cette colonne de liste.|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/fr/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) | Obtient la formule de la ligne des totaux de cette colonne de liste.|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/fr/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | Obtient la formule de cette colonne de liste.|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/fr/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) | Définit la formule pour cette colonne de liste.|



###  Exemples

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(4):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
listColumn = table.list_columns[4]
listColumn.totals_calculation = TotalsCalculation.SUM
listColumn.formula = "=[A]"
workbook.save(r"Book1.xlsx")

```

###  Voir également
* module [aspose.cells.tables](..)
