---
title: MsoLineFormat.DashStyle
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Gets or sets the dash style for the specified line
type: docs
url: /net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Gets or sets the dash style for the specified line.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Examples

```csharp
// Called: radio1.LineFormat.DashStyle = MsoLineDashStyle.Solid;
public static void MsoLineFormat_Property_DashStyle()
        {
            // Instantiate a new Workbook.
            Workbook workbook = new Workbook();

            // Add a group box to the first worksheet.
            GroupBox box = workbook.Worksheets[0].Shapes.AddGroupBox(1, 0, 1, 0, 300, 250);

            // Set the caption of the group box.
            box.Text = "Age Groups";
            box.Placement = PlacementType.FreeFloating;

            // Make it a 2-D box.
            box.Shadow = false;

            // Add a radio button.
            RadioButton radio1 = workbook.Worksheets[0].Shapes.AddRadioButton(3, 0, 2, 0, 30, 110);

            // Set its text string.
            radio1.Text = "20-29";

            // Set A1 cell as a linked cell for the radio button.
            radio1.LinkedCell = "A1";

            // Make the radio button 3-D.
            radio1.Shadow = true;

            // Set the foreground color of the radio button.
            radio1.FillFormat.ForeColor = Color.LightGreen;

            // Set the line style of the radio button.
            radio1.LineFormat.Style = MsoLineStyle.ThickThin;

            // Set the weight of the radio button.
            radio1.LineFormat.Weight = 4;

            // Set the line color of the radio button.
            radio1.LineFormat.ForeColor = Color.Blue;

            // Set the dash style of the radio button.
            radio1.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Make the line format visible.
            radio1.LineFormat.IsVisible = true;

            // Make the fill format visible.
            radio1.FillFormat.IsVisible = true;

            // Add another radio button.
            RadioButton radio2 = workbook.Worksheets[0].Shapes.AddRadioButton(6, 0, 2, 0, 30, 110);

            // Set its text string.
            radio2.Text = "30-39";

            // Set A1 cell as a linked cell for the radio button.
            radio2.LinkedCell = "A1";

            // Make the radio button 3-D.
            radio2.Shadow = true;

            // Set the foreground color of the radio button.
            radio2.FillFormat.ForeColor = Color.LightGreen;

            // Set the line style of the radio button.
            radio2.LineFormat.Style = MsoLineStyle.ThickThin;

            // Set the weight of the radio button.
            radio2.LineFormat.Weight = 4;

            // Set the line color of the radio button.
            radio2.LineFormat.ForeColor = Color.Blue;

            // Set the dash style of the radio button.
            radio2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Make the line format visible.
            radio2.LineFormat.IsVisible = true;

            // Make the fill format visible.
            radio2.FillFormat.IsVisible = true;

            // Add another radio button.
            RadioButton radio3 = workbook.Worksheets[0].Shapes.AddRadioButton(9, 0, 2, 0, 30, 110);

            // Set its text string.
            radio3.Text = "40-49";

            // Set A1 cell as a linked cell for the radio button.
            radio3.LinkedCell = "A1";

            // Make the radio button 3-D.
            radio3.Shadow = true;

            // Set the foreground color of the radio button.
            radio3.FillFormat.ForeColor = Color.LightGreen;

            // Set the line style of the radio button.
            radio3.LineFormat.Style = MsoLineStyle.ThickThin;

            // Set the weight of the radio button.
            radio3.LineFormat.Weight = 4;

            // Set the line color of the radio button.
            radio3.LineFormat.ForeColor = Color.Blue;

            // Set the dash style of the radio button.
            radio3.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Make the line format visible.
            radio3.LineFormat.IsVisible = true;

            // Make the fill format visible.
            radio3.FillFormat.IsVisible = true;

            // Get the shapes.
            Shape[] shapeObjects = new Shape[] { box, radio1, radio2, radio3 };

            // Group the shapes.
            GroupShape group = workbook.Worksheets[0].Shapes.Group(shapeObjects);

            // Save the excel file.
            workbook.Save("GroupShapeExample.xlsx");
            workbook.Save("GroupShapeExample.pdf");
        }
```

### See Also

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


