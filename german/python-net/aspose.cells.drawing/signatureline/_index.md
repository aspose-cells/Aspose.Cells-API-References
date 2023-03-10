---
title: SignatureLine Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 640
url: /de/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine Klasse
Stellen Sie die Signaturzeile dar.



Der Typ SignatureLine macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [SignatureLine()](/cells/de/python-net/aspose.cells.drawing/signatureline/__init__/#) | Erstellt eine neue Instanz von SignatureLine|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [id](/cells/de/python-net/aspose.cells.drawing/signatureline/id) | Ruft den Bezeichner für diese Signaturzeile ab oder legt ihn fest.|
| [provider_id](/cells/de/python-net/aspose.cells.drawing/signatureline/provider_id) | Ruft die ID des Signaturanbieters ab und legt sie fest.|
| [signer](/cells/de/python-net/aspose.cells.drawing/signatureline/signer) | Ruft den Unterzeichner ab und legt ihn fest.|
| [title](/cells/de/python-net/aspose.cells.drawing/signatureline/title) | Ruft den Titel des Sängers ab und legt ihn fest.|
| [email](/cells/de/python-net/aspose.cells.drawing/signatureline/email) | Ruft die E-Mail-Adresse des Sängers ab und legt sie fest.|
| [is_line](/cells/de/python-net/aspose.cells.drawing/signatureline/is_line) | Gibt an, ob es sich um eine Signaturzeile handelt.|
| [allow_comments](/cells/de/python-net/aspose.cells.drawing/signatureline/allow_comments) | Gibt an, ob Kommentare angehängt werden können.|
| [show_signed_date](/cells/de/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Gibt an, ob signiertes Datum angezeigt wird.|
| [instructions](/cells/de/python-net/aspose.cells.drawing/signatureline/instructions) | Ruft den Text ab, der dem Benutzer beim Signieren angezeigt wird, und legt ihn fest.|



###  Beispiel

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.drawing](..)
