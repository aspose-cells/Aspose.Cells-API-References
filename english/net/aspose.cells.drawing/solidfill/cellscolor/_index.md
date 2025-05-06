---
title: SolidFill.CellsColor
second_title: Aspose.Cells for .NET API Reference
description: SolidFill property. Gets and sets the CellsColor object
type: docs
url: /net/aspose.cells.drawing/solidfill/cellscolor/
---
## SolidFill.CellsColor property

Gets and sets the `CellsColor` object.

```csharp
public CellsColor CellsColor { get; set; }
```

### Examples

```csharp
// Called: shape.Fill.SolidFill.CellsColor.Color = fillColor;
public static void Property_CellsColor(
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


