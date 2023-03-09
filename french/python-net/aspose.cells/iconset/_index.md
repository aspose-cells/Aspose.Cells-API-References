---
title: IconSet classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 900
url: /fr/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet classe
 Décrivez la règle de mise en forme conditionnelle IconSet.
Cette règle de mise en forme conditionnelle applique des icônes aux cellules
selon leurs valeurs.



Le type IconSet expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [cf_icons](/cells/fr/python-net/aspose.cells/iconset/cf_icons) | Obtenez le [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon) de la collection|
| [cfvos](/cells/fr/python-net/aspose.cells/iconset/cfvos) | Obtenez l'instance CFValueObjects.|
| [type](/cells/fr/python-net/aspose.cells/iconset/type) | Obtenez ou définissez le type de jeu d'icônes à afficher.<br/>Le réglage du type vérifiera automatiquement si le nombre actuel de Cfvos est<br/> accord avec le nouveau type. Sinon, les anciens Cfvo seront nettoyés et<br/> les Cfvos par défaut seront ajoutés.|
| [is_custom](/cells/fr/python-net/aspose.cells/iconset/is_custom) | Indique si le jeu d'icônes est personnalisé.<br/> La valeur par défaut est faux.|
| [show_value](/cells/fr/python-net/aspose.cells/iconset/show_value) | Obtenez ou définissez le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles ce jeu d'icônes est appliqué.<br/> La valeur par défaut est true.|
| [reverse](/cells/fr/python-net/aspose.cells/iconset/reverse) | Obtenez ou définissez l'indicateur indiquant s'il faut inverser l'ordre par défaut des icônes dans ce jeu d'icônes.<br/> La valeur par défaut est faux.|



###  Exemples

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Voir également
* module [aspose.cells](..)
* classe [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon)
