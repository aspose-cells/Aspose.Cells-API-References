---
title: "License Class"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Cells for Python via Java"
description: "Provides methods to license the component."
type: docs
weight: 3290
url: /python-java/asposecells.api/license/
---

## License class

Provides methods to license the component.

## Constructors

| Name | Description |
| --- | --- |
| [License](#constructor) | Initializes a new instance of this class. |

## Methods

| Name | Description |
| --- | --- |
| [setLicense](#setlicense) | Licenses the component.

Tries to find the license in the following locations: 1. Explicit path. 2. The current working  |

### License() {#constructor}

Initializes a new instance of this class.

### setLicense(licenseName) (1 of 2) {#setlicense}

Licenses the component.

Tries to find the license in the following locations: 1. Explicit path. 2. The current working directory of the java application. 3. The folder that contains the Aspose component JAR file. 4. The folder that contains the client's calling JAR file.

---

### setLicense(byte_array) (2 of 2) {#setlicense-1}

Licenses the component.

Use this method to load a license from a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| byte_array | bytes | The byte array |

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

lic = License()
with open('Aspose.Cells.lic', 'rb') as f:
    lic.setLicense(f.read())

wb = Workbook()
wb.save("wb.xlsx")

jpype.shutdownJVM()
```
