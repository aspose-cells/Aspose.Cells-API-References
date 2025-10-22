##provider_id property
## provider_id property
Gets or sets the id of signature provider.
### Remarks
It's typically the CLSID of the provider com add-in.
### Example
```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4
#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx")
```
### Definition:
```python
@property
def provider_id(self):
...
@provider_id.setter
def provider_id(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`SignatureLine`](/cells/python-net/aspose.cells.drawing/signatureline)
