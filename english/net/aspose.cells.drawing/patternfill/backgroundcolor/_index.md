---
title: PatternFill.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets or sets the background Color of the Area
type: docs
url: /net/aspose.cells.drawing/patternfill/backgroundcolor/
---
## PatternFill.BackgroundColor property

Gets or sets the background Color of the [`Area`](../../area/).

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Green;
public static void PatternFill_Property_BackgroundColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Add a shape to the worksheet
            Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);

            // Set the fill format of the shape to AutomaticFill
            shape.Fill.FillType = FillType.Automatic;

            // Save the workbook
            workbook.Save("AutomaticFillDemo.xlsx");

            shape.Fill.FillType = FillType.Pattern;
            shape.Fill.Pattern = FillPattern.SolidDiamond;
            shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Red;
            shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Green;

            workbook.Save("PatternFillDemo2.xlsx");
            workbook.Save("PatternFillDemo2.pdf");
        }
```

### See Also

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


