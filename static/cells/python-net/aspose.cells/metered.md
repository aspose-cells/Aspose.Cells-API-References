##Metered class
## Metered class
Provides methods to set metered key.
The Metered type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/metered/__init__/#) | Initializes a new instance of this class. |
### Methods
| Method | Description |
| :- | :- |
| [`set_metered_key(self, public_key, private_key)`](/cells/python-net/aspose.cells/metered/set_metered_key/#system.string-system.string) | Sets metered public and private key.
| [`get_consumption_quantity()`](/cells/python-net/aspose.cells/metered/get_consumption_quantity/#) | Gets consumption file size |
| [`get_consumption_credit()`](/cells/python-net/aspose.cells/metered/get_consumption_credit/#) | Gets consumption credit |
| [`get_product_name(self)`](/cells/python-net/aspose.cells/metered/get_product_name/#) | Gets product name |
| [`is_metered_licensed()`](/cells/python-net/aspose.cells/metered/is_metered_licensed/#) | Check whether metered is licensed |
### Example
In this example, an attempt will be made to set metered public and private key
```python
from aspose.cells import Metered
matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")
```
### See Also
* module [`aspose.cells`](..)
