---
title: Hyperlink Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 790
url: /de/python-net/aspose.cells/hyperlink/
is_root: false
---
##  Hyperlink Klasse
Kapselt das Objekt, das einen Hyperlink darstellt.



Der Typ Hyperlink macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [address](/cells/de/python-net/aspose.cells/hyperlink/address) | Stellt die Adresse eines Hyperlinks dar.|
| [text_to_display](/cells/de/python-net/aspose.cells/hyperlink/text_to_display) | Stellt den Text dar, der für den angegebenen Hyperlink angezeigt werden soll.|
| [area](/cells/de/python-net/aspose.cells/hyperlink/area) | Ruft den Bereich der Hyperlinks ab.|
| [screen_tip](/cells/de/python-net/aspose.cells/hyperlink/screen_tip) | Gibt den QuickInfo-Text für den angegebenen Hyperlink zurück oder legt ihn fest.|
| [link_type](/cells/de/python-net/aspose.cells/hyperlink/link_type) | Ruft den Linktyp ab.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [delete()](/cells/de/python-net/aspose.cells/hyperlink/delete/#) | Löscht diesen Hyperlink|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells](..)
