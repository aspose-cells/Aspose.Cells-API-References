---
title: SignatureLine class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 640
url: /python-net/aspose.cells.drawing/signatureline/
is_root: false
---

## SignatureLine class

Represent the signature line.



The SignatureLine type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [SignatureLine()](/cells/python-net/aspose.cells.drawing/signatureline/__init__/#) | Constructs a new instance of SignatureLine |


### Properties
| Property | Description |
| :- | :- |
| [id](/cells/python-net/aspose.cells.drawing/signatureline/id) | Gets or sets identifier for this signature line. |
| [provider_id](/cells/python-net/aspose.cells.drawing/signatureline/provider_id) | Gets and sets the id of signature provider. |
| [signer](/cells/python-net/aspose.cells.drawing/signatureline/signer) | Gets and sets the signer. |
| [title](/cells/python-net/aspose.cells.drawing/signatureline/title) | Gets and sets the title of singer. |
| [email](/cells/python-net/aspose.cells.drawing/signatureline/email) | Gets and sets the email of singer. |
| [is_line](/cells/python-net/aspose.cells.drawing/signatureline/is_line) | Indicates whether it is a signature line. |
| [allow_comments](/cells/python-net/aspose.cells.drawing/signatureline/allow_comments) | Indicates whether comments could be attached. |
| [show_signed_date](/cells/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Indicates whether show signed date. |
| [instructions](/cells/python-net/aspose.cells.drawing/signatureline/instructions) | Gets and sets the text shown to user at signing time. |



### Example 


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
### See Also

* module [aspose.cells.drawing](../)
