---
title: SignatureLine klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 640
url: /sv/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine klass
Representera signaturlinjen.



Typen SignatureLine avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [SignatureLine()](/cells/sv/python-net/aspose.cells.drawing/signatureline/__init__/#) | Konstruerar en ny instans av SignatureLine|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [id](/cells/sv/python-net/aspose.cells.drawing/signatureline/id) | Hämtar eller ställer in identifierare för denna signaturrad.|
| [provider_id](/cells/sv/python-net/aspose.cells.drawing/signatureline/provider_id) | Hämtar och ställer in id för signaturleverantör.|
| [signer](/cells/sv/python-net/aspose.cells.drawing/signatureline/signer) | Får och ställer in undertecknaren.|
| [title](/cells/sv/python-net/aspose.cells.drawing/signatureline/title) | Får och sätter titeln sångare.|
| [email](/cells/sv/python-net/aspose.cells.drawing/signatureline/email) | Får och ställer in sångarens e-post.|
| [is_line](/cells/sv/python-net/aspose.cells.drawing/signatureline/is_line) | Indikerar om det är en signaturrad.|
| [allow_comments](/cells/sv/python-net/aspose.cells.drawing/signatureline/allow_comments) | Anger om kommentarer kan bifogas.|
| [show_signed_date](/cells/sv/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Anger om visa undertecknat datum.|
| [instructions](/cells/sv/python-net/aspose.cells.drawing/signatureline/instructions) | Hämtar och ställer in texten som visas för användaren vid undertecknandet.|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](..)
