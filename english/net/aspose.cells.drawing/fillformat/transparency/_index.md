---
title: FillFormat.Transparency
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: lineFmt.Transparency = 0.5;
public static void Property_Transparency()
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
            workbook.Save(&quot;LineFormatExample.xlsx&quot;);
            workbook.Save(&quot;LineFormatExample.pdf&quot;);
        }
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


