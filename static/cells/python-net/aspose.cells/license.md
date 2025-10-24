##License class
## License class
Provides methods to license the component.
The License type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/license/__init__/#) | Initializes a new instance of this class. |
### Methods
| Method | Description |
| :- | :- |
| [`set_license(self, license_name)`](/cells/python-net/aspose.cells/license/set_license/#system.string) | Licenses the component. |
| [`set_license(self, stream)`](/cells/python-net/aspose.cells/license/set_license/#io.rawiobase) | Licenses the component. |
### Example
In this example, an attempt will be made to find a license file named MyLicense.lic
in the folder that contains
the component, in the folder that contains the calling assembly,
in the folder of the entry assembly and then in the embedded resources of the calling assembly.
```python
from aspose.cells import License
license = License()
license.set_license("MyLicense.lic")
```
### See Also
* module [`aspose.cells`](..)
