---
title: FindOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 630
url: /fr/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions classe
Représente les options de recherche.



Le type FindOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [FindOptions()](/cells/fr/python-net/aspose.cells/findoptions/__init__/#) | Construit une nouvelle instance de FindOptions|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_case_sensitive](/cells/fr/python-net/aspose.cells/findoptions/is_case_sensitive) | Indique si la chaîne recherchée est sensible à la casse.|
| [case_sensitive](/cells/fr/python-net/aspose.cells/findoptions/case_sensitive) | Indique si la chaîne recherchée est sensible à la casse.|
| [look_at_type](/cells/fr/python-net/aspose.cells/findoptions/look_at_type) | Regardez le genre.|
| [is_range_set](/cells/fr/python-net/aspose.cells/findoptions/is_range_set) | Indique si la plage recherchée est définie.|
| [search_next](/cells/fr/python-net/aspose.cells/findoptions/search_next) | Ordre de recherche. Vrai : rechercher ensuite. Faux : recherche précédente.|
| [search_backward](/cells/fr/python-net/aspose.cells/findoptions/search_backward) | Si la recherche en arrière pour les cellules.|
| [seach_order_by_rows](/cells/fr/python-net/aspose.cells/findoptions/seach_order_by_rows) | Indique si la recherche est ordonnée par lignes ou par colonnes.|
| [look_in_type](/cells/fr/python-net/aspose.cells/findoptions/look_in_type) | Regardez dans le type.|
| [regex_key](/cells/fr/python-net/aspose.cells/findoptions/regex_key) | Indique si la clé recherchée est une expression régulière.<br/> Si vrai, la clé recherchée sera prise comme regex et analysée. Sinon, la clé sera analysée selon les règles de ms excel.|
| [value_type_sensitive](/cells/fr/python-net/aspose.cells/findoptions/value_type_sensitive) | Indique si le type de valeur de la cellule recherchée doit être identique à la clé recherchée.|
| [style](/cells/fr/python-net/aspose.cells/findoptions/style) | Le format à rechercher.|
| [convert_numeric_data](/cells/fr/python-net/aspose.cells/findoptions/convert_numeric_data) | Obtient ou définit une valeur qui indique si la valeur de chaîne recherchée est convertie en données numériques.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_range()](/cells/fr/python-net/aspose.cells/findoptions/get_range/#) | Obtient et définit la plage recherchée.|
| [set_range(ca)](/cells/fr/python-net/aspose.cells/findoptions/set_range/#CellArea) | Définit la plage recherchée.|



###  Exemple

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Voir également
* module [aspose.cells](..)
