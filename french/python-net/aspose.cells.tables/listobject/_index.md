---
title: ListObject classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject classe
Représente un objet de liste dans une feuille de calcul.
 L'objet ListObject est membre de la collection ListObjects.
La collection ListObjects contient tous les objets de liste d'une feuille de calcul.



Le type ListObject expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [start_row](/cells/fr/python-net/aspose.cells.tables/listobject/start_row) | Obtient la ligne de début de la plage.|
| [start_column](/cells/fr/python-net/aspose.cells.tables/listobject/start_column) | Obtient la colonne de début de la plage.|
| [end_row](/cells/fr/python-net/aspose.cells.tables/listobject/end_row) | Obtient la dernière ligne de la plage.|
| [end_column](/cells/fr/python-net/aspose.cells.tables/listobject/end_column) |Obtient la colonne de fin de la plage.|
| [list_columns](/cells/fr/python-net/aspose.cells.tables/listobject/list_columns) | Obtient ListColumns de ListObject.|
| [show_header_row](/cells/fr/python-net/aspose.cells.tables/listobject/show_header_row) | Obtient et définit si ce ListObject affiche la ligne d'en-tête.|
| [show_totals](/cells/fr/python-net/aspose.cells.tables/listobject/show_totals) | Obtient et définit si ce ListObject affiche la ligne totale.|
| [data_range](/cells/fr/python-net/aspose.cells.tables/listobject/data_range) | Obtient la plage de données de ListObject.|
| [query_table](/cells/fr/python-net/aspose.cells.tables/listobject/query_table) | Obtient le QueryTable lié.|
| [data_source_type](/cells/fr/python-net/aspose.cells.tables/listobject/data_source_type) | Obtient le type de source de données de la table.|
| [auto_filter](/cells/fr/python-net/aspose.cells.tables/listobject/auto_filter) | Obtient le filtre automatique.|
| [display_name](/cells/fr/python-net/aspose.cells.tables/listobject/display_name) | Obtient et définit le nom d'affichage.|
| [comment](/cells/fr/python-net/aspose.cells.tables/listobject/comment) | Obtient et définit le commentaire de la table.|
| [show_table_style_first_column](/cells/fr/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Indique si le style doit être appliqué à la première colonne du tableau.|
| [show_table_style_last_column](/cells/fr/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Indique si la dernière colonne du tableau doit avoir le style appliqué.|
| [show_table_style_row_stripes](/cells/fr/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Indique si la mise en forme des bandes de ligne est appliquée.|
| [show_table_style_column_stripes](/cells/fr/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Indique si la mise en forme des bandes de colonnes est appliquée.|
| [table_style_type](/cells/fr/python-net/aspose.cells.tables/listobject/table_style_type) | Gets et le style de tableau intégré.|
| [table_style_name](/cells/fr/python-net/aspose.cells.tables/listobject/table_style_name) | Obtient et définit le nom du style de tableau.|
| [xml_map](/cells/fr/python-net/aspose.cells.tables/listobject/xml_map) | Obtient un [ListObject.xml_map](/cells/fr/python-net/aspose.cells.tables/listobject#xml_map) utilisé pour cette liste.|
| [alternative_text](/cells/fr/python-net/aspose.cells.tables/listobject/alternative_text) | Obtient et définit le texte alternatif.|
| [alternative_description](/cells/fr/python-net/aspose.cells.tables/listobject/alternative_description) | Obtient et définit la description alternative.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [convert_to_range()](/cells/fr/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Convertissez le tableau en plage.|
| [convert_to_range(options)](/cells/fr/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Convertissez le tableau en plage.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/fr/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Redimensionnez la plage de l'objet de liste.|
| [put_cell_value(row_offset, column_offset, value)](/cells/fr/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Mettez la valeur dans la cellule.|
| [update_column_name()](/cells/fr/python-net/aspose.cells.tables/listobject/update_column_name/#) |Met à jour le nom de toutes les colonnes de la liste à partir de la feuille de calcul.|
| [filter()](/cells/fr/python-net/aspose.cells.tables/listobject/filter/#) | Filtrez le tableau.|
| [apply_style_to_range()](/cells/fr/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Appliquez le style de tableau à la plage.|



###  Exemple

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  Voir également
* module [aspose.cells.tables](..)
