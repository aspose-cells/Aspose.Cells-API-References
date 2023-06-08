---
title: Row.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Row method. Gets the style of this row
type: docs
url: /net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Gets the style of this row.

```csharp
public Style GetStyle()
```

### Remarks

Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this row. Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### See Also

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


