##add_signature_line method
## add_signature_line(self, upper_left_row, upper_left_column, signature_line) {#int-int-aspose.cells.drawing.SignatureLine}
Adds a Signature Line to the worksheet.
### Returns
```python
def add_signature_line(self, upper_left_row, upper_left_column, signature_line):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| signature_line | aspose.cells.drawing.SignatureLine | Represents a signature line object. |
### Example
```python
from aspose.cells.drawing import SignatureLine
wSignatureLine = SignatureLine()
wSignatureLine.allow_comments = True
wSignatureLine.email = "example@example.com"
wSignatureLine.instructions = "Sign to confirm the excel content."
wSignatureLine.is_line = True
wSignatureLine.show_signed_date = True
wSignatureLine.signer = "User"
wSignatureLine.title = "tester"
# wSignatureLine.SignatureLineType = SignatureType.Stamp;
signatureLine1 = shapes.add_signature_line(0, 0, wSignatureLine)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
