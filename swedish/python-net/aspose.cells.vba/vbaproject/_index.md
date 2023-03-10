---
title: VbaProject klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  VbaProject klass
Representerar VBA-projektet.



Typen VbaProject avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_valid_signed](/cells/sv/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Indikerar om signaturen för VBA-projektet är giltig eller inte.|
| [cert_raw_data](/cells/sv/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Får certifikatrådata om detta VBA-projekt är signerat.|
| [name](/cells/sv/python-net/aspose.cells.vba/vbaproject/name) | Hämtar och ställer in namnet på VBA-projektet.|
| [is_signed](/cells/sv/python-net/aspose.cells.vba/vbaproject/is_signed) | Indikerar om VBA-koden är signerad eller inte.|
| [is_protected](/cells/sv/python-net/aspose.cells.vba/vbaproject/is_protected) | Indikerar om detta VBA-projekt är skyddat.|
| [islocked_for_viewing](/cells/sv/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Indikerar om detta VBA-projekt är låst för visning.|
| [modules](/cells/sv/python-net/aspose.cells.vba/vbaproject/modules) | Får alla [VbaModule](/cells/sv/python-net/aspose.cells.vba/vbamodule) objekt.|
| [references](/cells/sv/python-net/aspose.cells.vba/vbaproject/references) | Får alla referenser av VBA-projekt.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [sign(digital_signature)](/cells/sv/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Signera detta VBA-projekt med en DigitalSignatur|
| [protect(islocked_for_viewing, password)](/cells/sv/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Skyddar eller avskyddar detta VBA-projekt.|
| [copy(source)](/cells/sv/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Kopiera VBA-projekt från annan fil.|
| [validate_password(password)](/cells/sv/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Validerar skyddslösenord.|



###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Se även
* modul [aspose.cells.vba](..)
* klass [VbaModule](/cells/sv/python-net/aspose.cells.vba/vbamodule)
