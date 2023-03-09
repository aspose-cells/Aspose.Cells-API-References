---
title: Hyperlink classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 790
url: /fr/python-net/aspose.cells/hyperlink/
is_root: false
---
##  Hyperlink classe
Encapsule l'objet qui représente un lien hypertexte.



Le type Hyperlink expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [address](/cells/fr/python-net/aspose.cells/hyperlink/address) | Représente l'adresse d'un lien hypertexte.|
| [text_to_display](/cells/fr/python-net/aspose.cells/hyperlink/text_to_display) | Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte.|
| [area](/cells/fr/python-net/aspose.cells/hyperlink/area) | Obtient la plage de liens hypertexte.|
| [screen_tip](/cells/fr/python-net/aspose.cells/hyperlink/screen_tip) | Renvoie ou définit le texte de l'info-bulle pour le lien hypertexte spécifié.|
| [link_type](/cells/fr/python-net/aspose.cells/hyperlink/link_type) | Obtient le type de lien.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [delete()](/cells/fr/python-net/aspose.cells/hyperlink/delete/#) | Supprime ce lien hypertexte|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Adding a hyperlink to a URL at "A1" cell
index = worksheet.hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Getting a Hyperlink by index.
hyperlink = worksheet.hyperlinks[index]
# Setting display text of this hyperlink.
hyperlink.text_to_display = "Aspose"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells](..)
