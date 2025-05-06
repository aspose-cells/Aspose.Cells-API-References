---
title: MsoLineFormat.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Gets and sets the border line back color
type: docs
url: /net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Gets and sets the border line back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
// Called: lineFormat.BackColor = Color.Blue;
public static void Property_BackColor()
        {
            // Instantiate a new Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an arc shape to the worksheet
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Get the MsoLineFormat object from the shape
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Set properties of the MsoLineFormat object
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Save the workbook
            workbook.Save(&quot;MsoLineFormatExample.xlsx&quot;);
        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


