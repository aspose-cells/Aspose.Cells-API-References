---
title: Aspose::Cells::Row::GetStyle method
linktitle: GetStyle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Row::GetStyle method. Gets the style of this row in C++.'
type: docs
weight: 2100
url: /cpp/aspose.cells/row/getstyle/
---
## Row::GetStyle method


Gets the style of this row.

```cpp
Style Aspose::Cells::Row::GetStyle()
```

## Remarks


Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call ApplyStyle(Style, StyleFlag) or SetStyle(Style) method to apply the change to this row.
[Row](../)'s style is the style which will be inherited by cells in this row(those cells that have no custom style settings,
such as existing cells that have not been set style explicitly, or those that have not been instantiated) 
## See Also

* Class [Style](../../style/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
