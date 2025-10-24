##SignatureLine class
## SignatureLine class
Represent the signature line.
The SignatureLine type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells.drawing/signatureline/__init__/#) | Constructs a new instance of SignatureLine |
### Properties
| Property | Description |
| :- | :- |
| [id](/cells/python-net/aspose.cells.drawing/signatureline/id) | Gets or sets identifier for this signature line. |
| [provider_id](/cells/python-net/aspose.cells.drawing/signatureline/provider_id) | Gets or sets the id of signature provider. |
| [signer](/cells/python-net/aspose.cells.drawing/signatureline/signer) | Gets or sets the signer. |
| [title](/cells/python-net/aspose.cells.drawing/signatureline/title) | Gets or sets the title of singer. |
| [email](/cells/python-net/aspose.cells.drawing/signatureline/email) | Gets or sets the email of singer. |
| [is_line](/cells/python-net/aspose.cells.drawing/signatureline/is_line) | Indicates whether it is a signature line. |
| [allow_comments](/cells/python-net/aspose.cells.drawing/signatureline/allow_comments) | Indicates whether comments could be attached. |
| [show_signed_date](/cells/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Indicates whether show signed date. |
| [instructions](/cells/python-net/aspose.cells.drawing/signatureline/instructions) | Gets or sets the text shown to user at signing time. |
| [signature_line_type](/cells/python-net/aspose.cells.drawing/signatureline/signature_line_type) | Gets or sets the signature type.
### Example
```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine
# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon"
s.title = "Development"
s.email = "simon@aspose.com"
s.instructions = "Sign to confirm the excel content."
#  Adds a Signature Line to the worksheet.
signatureLine = worksheet.shapes.add_signature_line(0, 0, s)
# do your business
# Save the excel file.
workbook.save("result.xlsx")
```
### See Also
* module [`aspose.cells.drawing`](..)
