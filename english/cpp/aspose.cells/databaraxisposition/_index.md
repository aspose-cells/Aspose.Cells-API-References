﻿---
title: Aspose::Cells::DataBarAxisPosition enum
linktitle: DataBarAxisPosition
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DataBarAxisPosition enum. Specifies the axis position for a range of cells with conditional formatting as data bars in C++.'
type: docs
weight: 19100
url: /cpp/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enum


Specifies the axis position for a range of cells with conditional formatting as data bars.

```cpp
enum class DataBarAxisPosition
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Automatic | 0 | <br>Display the axis at a variable position based on the ratio of the minimum negative value to the maximum positive value in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction. When all values are positive or all values are negative, no axis is displayed. |
| Midpoint | 1 | <br>Display the axis at the midpoint of the cell regardless of the set of values in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction. |
| None | 2 | <br>No axis is displayed, and both positive and negative values are displayed in the left-to-right direction. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
