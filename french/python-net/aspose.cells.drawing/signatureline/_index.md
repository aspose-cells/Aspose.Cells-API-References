---
title: SignatureLine classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 640
url: /fr/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine classe
Représente la ligne de signature.



Le type SignatureLine expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [SignatureLine()](/cells/fr/python-net/aspose.cells.drawing/signatureline/__init__/#) | Construit une nouvelle instance de SignatureLine|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [id](/cells/fr/python-net/aspose.cells.drawing/signatureline/id) | Obtient ou définit l'identifiant de cette ligne de signature.|
| [provider_id](/cells/fr/python-net/aspose.cells.drawing/signatureline/provider_id) | Obtient et définit l'ID du fournisseur de signature.|
| [signer](/cells/fr/python-net/aspose.cells.drawing/signatureline/signer) | Obtient et définit le signataire.|
| [title](/cells/fr/python-net/aspose.cells.drawing/signatureline/title) | Obtient et définit le titre du chanteur.|
| [email](/cells/fr/python-net/aspose.cells.drawing/signatureline/email) | Obtient et définit l'e-mail du chanteur.|
| [is_line](/cells/fr/python-net/aspose.cells.drawing/signatureline/is_line) | Indique s'il s'agit d'une ligne de signature.|
| [allow_comments](/cells/fr/python-net/aspose.cells.drawing/signatureline/allow_comments) | Indique si des commentaires peuvent être joints.|
| [show_signed_date](/cells/fr/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Indique si afficher la date signée.|
| [instructions](/cells/fr/python-net/aspose.cells.drawing/signatureline/instructions) | Obtient et définit le texte affiché à l'utilisateur au moment de la signature.|



###  Exemple

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

###  Voir également
* module [aspose.cells.drawing](..)
