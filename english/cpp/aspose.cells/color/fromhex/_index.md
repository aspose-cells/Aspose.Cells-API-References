---
title: Aspose::Cells::Color::FromHex method
linktitle: FromHex
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Color::FromHex method. Creates a Color from a hexadecimal color string in C++.'
type: docs
weight: 300
url: /cpp/aspose.cells/color/fromhex/
---
## Color::FromHex method


Creates a [Color](../) from a hexadecimal color string.

```cpp
static Color Aspose::Cells::Color::FromHex(const U16String &hex)
```


| Parameter | Type | Description |
| --- | --- | --- |
| hex | const U16String\& | A UTF-16 string representing a color in hexadecimal format. Supported formats include **#RRGGBB**, **RRGGBB**, **#AARRGGBB**, and **AARRGGBB**. |

## ReturnValue

A [Color](../) structure that corresponds to the specified hexadecimal value.
## Remarks



If the alpha component is not specified, it defaults to 255 (fully opaque). 

## Examples


```cpp
auto c1 = Color::FromHex(u"#ff0000");   // a=255, r=255, g=0, b=0
auto c2 = Color::FromHex(u"80ff0000");  // a=128, r=255, g=0, b=0
```

## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
