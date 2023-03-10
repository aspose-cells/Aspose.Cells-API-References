---
title: License konstruktör
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells/license/__init__/
is_root: false
---
##  License() {#}
Initierar en ny instans av den här klassen.



```python
def __init__(self):
    ...
```



###  Exempel

I det här exemplet kommer ett försök att göras att hitta en licensfil med namnet MyLicense.lic
 i mappen som innehåller


komponenten, i mappen som innehåller den anropande församlingen,
i mappen för postförsamlingen och sedan i de inbäddade resurserna för den anropande församlingen.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```



###  Se även
* modul [aspose.cells](../../)
* klass [License](/cells/sv/python-net/aspose.cells/license)
