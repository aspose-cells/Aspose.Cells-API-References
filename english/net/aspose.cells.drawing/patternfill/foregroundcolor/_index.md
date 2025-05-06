---
title: PatternFill.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets or sets the foreground Color
type: docs
url: /net/aspose.cells.drawing/patternfill/foregroundcolor/
---
## PatternFill.ForegroundColor property

Gets or sets the foreground Color.

```csharp
public Color ForegroundColor { get; set; }
```

### Examples

```csharp
// Called: shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Red;
public static void Property_ForegroundColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);

            // Add a shape to the worksheet
            Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);

            // Set the fill format of the shape to AutomaticFill
            shape.Fill.FillType = FillType.Automatic;

            // Save the workbook
            workbook.Save(&quot;AutomaticFillDemo.xlsx&quot;);

            shape.Fill.FillType = FillType.Pattern;
            shape.Fill.Pattern = FillPattern.SolidDiamond;
            shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Red;
            shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Green;

            workbook.Save(&quot;PatternFillDemo2.xlsx&quot;);
            workbook.Save(&quot;PatternFillDemo2.pdf&quot;);
        }
```

### See Also

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


