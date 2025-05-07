---
title: MsoLineFormat.Transparency
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: lineFormat.Transparency = 0.5;
public static void Property_Transparency()
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
            workbook.Save("MsoLineFormatExample.xlsx");
        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


