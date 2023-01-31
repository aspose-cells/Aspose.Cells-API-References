---
title: License class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 980
url: /python-net/aspose.cells/license/
is_root: false
---

## License class

Provides methods to license the component.



The License type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [License()](/cells/python-net/aspose.cells/license/__init__/#) | Initializes a new instance of this class. |


### Methods
| Method | Description |
| :- | :- |
| [set_license(license_name)](/cells/python-net/aspose.cells/license/set_license/#str) | Licenses the component. |
| [set_license(stream)](/cells/python-net/aspose.cells/license/set_license/#io.RawIOBase) | Licenses the component. |


### Example 


In this example, an attempt will be made to find a license file named MyLicense.lic
in the folder that contains 


the component, in the folder that contains the calling assembly,
in the folder of the entry assembly and then in the embedded resources of the calling assembly.

```
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
### See Also

* module [aspose.cells](../)
