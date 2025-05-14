---
title: MsoFillFormat.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets and sets the file back color
type: docs
url: /net/aspose.cells.drawing/msofillformat/backcolor/
---
## MsoFillFormat.BackColor property

Gets and sets the file back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
// Called: fillFormat.BackColor = Color.LightBlue;
public static void MsoFillFormat_Property_BackColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an arc shape to the worksheet
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Access the fill format of the shape
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Set the fill fore color
            fillFormat.ForeColor = Color.Blue;

            // Set the fill back color
            fillFormat.BackColor = Color.LightBlue;

            // Set the transparency
            fillFormat.Transparency = 0.5;

            // Check if the fill is visible
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Set a one-color gradient fill
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Save the workbook
            workbook.Save("MsoFillFormatExample.xlsx");
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


