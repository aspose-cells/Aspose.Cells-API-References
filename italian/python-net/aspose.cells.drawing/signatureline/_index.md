---
title: classe SignatureLine
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 640
url: /it/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  classe SignatureLine
Rappresenta la riga della firma.



Il tipo SignatureLine espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [SignatureLine()](/cells/it/python-net/aspose.cells.drawing/signatureline/__init__/#) | Costruisce una nuova istanza di SignatureLine|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [id](/cells/it/python-net/aspose.cells.drawing/signatureline/id) | Ottiene o imposta l'identificatore per questa riga della firma.|
| [provider_id](/cells/it/python-net/aspose.cells.drawing/signatureline/provider_id) | Ottiene e imposta l'ID del provider della firma.|
| [signer](/cells/it/python-net/aspose.cells.drawing/signatureline/signer) | Ottiene e imposta il firmatario.|
| [title](/cells/it/python-net/aspose.cells.drawing/signatureline/title) | Ottiene e imposta il titolo del cantante.|
| [email](/cells/it/python-net/aspose.cells.drawing/signatureline/email) | Ottiene e imposta l'e-mail del cantante.|
| [is_line](/cells/it/python-net/aspose.cells.drawing/signatureline/is_line) | Indica se si tratta di una riga della firma.|
| [allow_comments](/cells/it/python-net/aspose.cells.drawing/signatureline/allow_comments) | Indica se è possibile allegare commenti.|
| [show_signed_date](/cells/it/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Indica se mostrare la data firmata.|
| [instructions](/cells/it/python-net/aspose.cells.drawing/signatureline/instructions) | Ottiene e imposta il testo mostrato all'utente al momento della firma.|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells.drawing](..)
