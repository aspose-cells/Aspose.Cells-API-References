---
title: Aspose::Cells::Column::GetStyle method
linktitle: GetStyle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Column::GetStyle method. Gets the style of this column in C++.'
type: docs
weight: 1500
url: /cpp/aspose.cells/column/getstyle/
---
## Column::GetStyle method


Gets the style of this column.

```cpp
Style Aspose::Cells::Column::GetStyle()
```

## Remarks


Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call ApplyStyle(Style, StyleFlag) or SetStyle(Style) method to apply the change to this column.
[Column](../)'s style is the style which will be inherited by cells in this column(those cells that have no custom style settings,
such as existing cells that have not been set style explicitly, or those that have not been instantiated) 
## See Also

* Class [Style](../../style/)
* Class [Column](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
