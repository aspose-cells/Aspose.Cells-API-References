---
title: Column.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Column method. Gets the style of this column
type: docs
url: /net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Gets the style of this column.

```csharp
public Style GetStyle()
```

### Remarks

Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this column. Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### See Also

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


