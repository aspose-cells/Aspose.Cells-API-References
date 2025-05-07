---
title: Border.Color
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets or sets the Color of the border
type: docs
url: /net/aspose.cells/border/color/
---
## Border.Color property

Gets or sets the Color of the border.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: style.Borders[BorderType.TopBorder].Color = Color.Red;
private Style Property_Color(Workbook workbook)
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

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


