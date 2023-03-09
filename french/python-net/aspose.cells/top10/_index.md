---
title: Top10 classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1480
url: /fr/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 classe
 Décrivez la règle de mise en forme conditionnelle Top10.
Cette règle de mise en forme conditionnelle met en évidence les cellules dont
les valeurs se situent dans la tranche N supérieure ou N inférieure, comme spécifié.



Le type Top10 expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [Top10()](/cells/fr/python-net/aspose.cells/top10/__init__/#) | Construit une nouvelle instance de Top10|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_percent](/cells/fr/python-net/aspose.cells/top10/is_percent) | Obtenir ou définir si une règle "top/bottom n" est une règle "top/bottom n percent".<br/> La valeur par défaut est faux.|
| [is_bottom](/cells/fr/python-net/aspose.cells/top10/is_bottom) | Obtenir ou définir si une règle "top/bottom n" est une règle "bottom n".<br/> La valeur par défaut est faux.|
| [rank](/cells/fr/python-net/aspose.cells/top10/rank) | Obtenez ou définissez la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n".<br/>Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100.<br/>Sinon il doit être compris entre 0 et 1000.<br/> La valeur par défaut est 10.|



###  Exemple

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  Voir également
* module [aspose.cells](..)
