﻿---
title: Aspose::Cells::Drawing::GradientFill::SetOneColorGradient method
linktitle: SetOneColorGradient
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::GradientFill::SetOneColorGradient method. Sets the specified fill to a one-color gradient. Only applies for Excel 2007 in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill::SetOneColorGradient method


Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

```cpp
void Aspose::Cells::Drawing::GradientFill::SetOneColorGradient(const Aspose::Cells::Color &color, double degree, GradientStyleType style, int32_t variant)
```


| Parameter | Type | Description |
| --- | --- | --- |
| color | const Aspose::Cells::Color\& | One gradient color. |
| degree | double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | GradientStyleType | Gradient shading style. |
| variant | int32_t | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [GradientStyleType](../../gradientstyletype/)
* Class [GradientFill](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
