---
title: SolidFill.Color
second_title: Aspose.Cells for .NET API Reference
description: SolidFill property. Gets or sets the Color
type: docs
url: /net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Gets or sets the Color.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: shape.Fill.SolidFill.Color = fillColor;
public static void SolidFill_Property_Color(
            Worksheet sheet,
            System.Drawing.Color fillColor,
            System.Drawing.Color textColor,
            string text)
        {
            var shape = sheet.Shapes[0];
            shape.LineFormat.ForeColor = fillColor;
            shape.Fill.SolidFill.CellsColor.Color = fillColor;
            shape.Fill.SolidFill.Color = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;
        }
```

### See Also

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


