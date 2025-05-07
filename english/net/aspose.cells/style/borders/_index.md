---
title: Style.Borders
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the BorderCollection of the style
type: docs
url: /net/aspose.cells/style/borders/
---
## Style.Borders property

Gets the [`BorderCollection`](../../bordercollection/) of the style.

```csharp
public BorderCollection Borders { get; }
```

### Examples

```csharp
// Called: style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
private Style Property_Borders(Workbook workbook)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].Color = Color.Blue;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].Color = Color.Green;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            return style;
        }
```

### See Also

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


