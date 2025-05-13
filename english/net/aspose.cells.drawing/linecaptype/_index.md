---
title: Enum LineCapType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.LineCapType enum. Represents the caps of a line
type: docs
url: /net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Represents the caps of a line

```csharp
public enum LineCapType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Square | `0` | Square protrudes by half line width. |
| Round | `1` | Rounded ends. |
| Flat | `2` | Line ends at end point. |
| None | `3` | None cap |

### Examples

```csharp
// Called: lineFmt.CapType = LineCapType.Flat;
public static void Drawing_Type_LineCapType()
        {
            // Instantiate a new Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Add a rectangle shape to the worksheet
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            LineFormat lineFmt = shape.Line;

            // Set various properties of the LineFormat
            lineFmt.CompoundType = MsoLineStyle.Single;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.JoinType = LineJoinType.Round;
            lineFmt.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.BeginArrowheadLength = MsoArrowheadLength.Long;
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadLength = MsoArrowheadLength.Long;
            lineFmt.Weight = 2.0d;

            // Set fill properties
            lineFmt.FillType = FillType.Solid;
            lineFmt.Transparency = 0.5;

            // Save the workbook
            workbook.Save("LineFormatExample.xlsx");
            workbook.Save("LineFormatExample.pdf");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


