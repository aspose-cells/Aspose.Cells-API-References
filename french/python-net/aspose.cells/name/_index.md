---
title: Name classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1070
url: /fr/python-net/aspose.cells/name/
is_root: false
---
##  Name classe
Représente un nom défini pour une plage de cellules.



Le type Name expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [comment](/cells/fr/python-net/aspose.cells/name/comment) | Obtient et définit le commentaire du nom.<br/> Ne s'applique qu'à Excel 2007.|
| [text](/cells/fr/python-net/aspose.cells/name/text) | Obtient le texte du nom de l'objet.|
| [full_text](/cells/fr/python-net/aspose.cells/name/full_text) | Obtient le nom en texte intégral de l'objet avec le paramètre d'étendue.|
| [refers_to](/cells/fr/python-net/aspose.cells/name/refers_to) | Renvoie ou définit la formule à laquelle le nom est défini pour faire référence, en commençant par un signe égal.|
| [r1c1_refers_to](/cells/fr/python-net/aspose.cells/name/r1c1_refers_to) | Obtient ou définit une référence R1C1 du [Name](/cells/fr/python-net/aspose.cells/name).|
| [is_referred](/cells/fr/python-net/aspose.cells/name/is_referred) | Indique si ce nom est référencé par d'autres formules.|
| [is_visible](/cells/fr/python-net/aspose.cells/name/is_visible) | Indique si le nom est visible.|
| [sheet_index](/cells/fr/python-net/aspose.cells/name/sheet_index) | Indique que ce nom appartient à Workbook ou Worksheet.<br/> 0 = nom global, sinon index de la feuille (base un)|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Obtenir la référence de ce Nom.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/fr/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Obtenez la référence de ce nom en fonction de la cellule spécifiée.|
| [get_ranges()](/cells/fr/python-net/aspose.cells/name/get_ranges/#) | Obtient toutes les plages référencées par ce nom.|
| [get_ranges(recalculate)](/cells/fr/python-net/aspose.cells/name/get_ranges/#bool) | Obtient toutes les plages référencées par ce nom.|
| [get_range()](/cells/fr/python-net/aspose.cells/name/get_range/#) | Obtient la plage si ce nom fait référence à une plage.|
| [get_range(recalculate)](/cells/fr/python-net/aspose.cells/name/get_range/#bool) | Obtient la plage si ce nom fait référence à une plage|
| [get_range(sheet_index, row, column)](/cells/fr/python-net/aspose.cells/name/get_range/#int-int-int) | Obtient la plage si ce nom fait référence à une plage.<br/> Si la référence de ce nom n'est pas absolue, la plage peut être différente pour différentes cellules.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | Définissez la référence de ce Nom.|
| [get_referred_areas(recalculate)](/cells/fr/python-net/aspose.cells/name/get_referred_areas/#bool) | Obtient toutes les références référencées par ce nom.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [Name](/cells/fr/python-net/aspose.cells/name)
