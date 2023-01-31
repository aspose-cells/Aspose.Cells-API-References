---
title: License constructor
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 10
url: /python-net/aspose.cells/license/__init__/
is_root: false
---

## License() {#}

Initializes a new instance of this class.



```python
def __init__(self):
    ...
```


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
* module [aspose.cells](../../)
* class [License](/cells/python-net/aspose.cells/license)
