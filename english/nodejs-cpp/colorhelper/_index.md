﻿---
title: ColorHelper
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Provides helper functions about color.
type: docs
url: /nodejs-cpp/colorhelper/
---

## ColorHelper class

Provides helper functions about color.

```javascript
class ColorHelper;
```


## Methods

| Method | Description |
| --- | --- |
| static [fromOleColor(number)](#fromOleColor-number-)| Convert OLE_COLOR. |
| static [toOleColor(Color, Workbook)](#toOleColor-color-workbook-)| Convert color to OLE_COLOR |


### fromOleColor(number) {#fromOleColor-number-}

Convert OLE_COLOR.

```javascript
static fromOleColor(oleColor: number) : Color;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oleColor | number | The value of OLE_COLOR. |

**Returns**

The [Color](./color/) object.

### toOleColor(Color, Workbook) {#toOleColor-color-workbook-}

Convert color to OLE_COLOR

```javascript
static toOleColor(color: Color, workbook: Workbook) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](./color/) | The [Color](./color/) object. |
| workbook | [Workbook](./workbook/) |  |

**Returns**

The value of OLE_COLOR


