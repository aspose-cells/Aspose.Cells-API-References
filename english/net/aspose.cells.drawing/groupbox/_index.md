---
title: GroupBox
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 2100
url: /net/aspose.cells.drawing/groupbox/
---
## GroupBox class

Encapsulates the object that represents a groupbox in a spreadsheet.

```csharp
public class GroupBox : Shape
```

## Properties

| Name | Description |
| --- | --- |
| [Shadow](shadow) { get; set; } | Indicates whether the groupbox has shadow. |

### Examples

```csharp

[C#]

//Instantiate a new Workbook.
Workbook excelbook = new Workbook();
 
//Add a group box to the first worksheet.
Aspose.Cells.GroupBox box = excelbook.Worksheets[0].Shapes.AddGroupBox(1, 0, 1, 0, 300, 250);
 
//Set the caption of the group box.
box.Text = "Age Groups";
box.Placement = PlacementType.FreeFloating;
 
//Make it 2-D box.
box.Shadow = false;
 
//Add a radio button.
Aspose.Cells.RadioButton radio1 = excelbook.Worksheets[0].Shapes.AddRadioButton(3, 0, 2, 0, 30, 110);
 
//Set its text string.
radio1.Text = "20-29";
 
//Set A1 cell as a linked cell for the radio button.
radio1.LinkedCell = "A1";
 
//Make the radio button 3-D.
radio1.Shadow = true;
 
//Set the foreground color of the radio button.
radio1.FillFormat.ForeColor = Color.LightGreen;
 
//Set the line style of the radio button.
radio1.LineFormat.Style = MsoLineStyle.ThickThin;
 
//Set the weight of the radio button.
radio1.LineFormat.Weight = 4;
 
//Set the line color of the radio button.
radio1.LineFormat.ForeColor = Color.Blue;
 
//Set the dash style of the radio button.
radio1.LineFormat.DashStyle = MsoLineDashStyle.Solid;
 
//Make the line format visible.
radio1.LineFormat.IsVisible = true;
 
//Make the fill format visible.
radio1.FillFormat.IsVisible = true;
 
//Add another radio button.
Aspose.Cells.RadioButton radio2 = excelbook.Worksheets[0].Shapes.AddRadioButton(6, 0, 2, 0, 30, 110);
 
//Set its text string.
radio2.Text = "30-39";
 
//Set A1 cell as a linked cell for the radio button.
radio2.LinkedCell = "A1";
 
//Make the radio button 3-D.
radio2.Shadow = true;
 
//Set the foreground color of the radio button.
radio2.FillFormat.ForeColor = Color.LightGreen;
 
//Set the line style of the radio button.
radio2.LineFormat.Style = MsoLineStyle.ThickThin;
 
//Set the weight of the radio button.
radio2.LineFormat.Weight = 4;
 
//Set the line color of the radio button.
radio2.LineFormat.ForeColor = Color.Blue;
 
//Set the dash style of the radio button.
radio2.LineFormat.DashStyle = MsoLineDashStyle.Solid;
 
//Make the line format visible.
radio2.LineFormat.IsVisible = true;
 
//Make the fill format visible.
radio2.FillFormat.IsVisible = true;
 
//Add another radio button.
Aspose.Cells.RadioButton radio3 = excelbook.Worksheets[0].Shapes.AddRadioButton(9, 0, 2, 0, 30, 110);
 
//Set its text string.
radio3.Text = "40-49";
 
//Set A1 cell as a linked cell for the radio button.
radio3.LinkedCell = "A1";
 
//Make the radio button 3-D.
radio3.Shadow = true;
 
//Set the foreground color of the radio button.
radio3.FillFormat.ForeColor = Color.LightGreen;
 
//Set the line style of the radio button.
radio3.LineFormat.Style = MsoLineStyle.ThickThin;
 
//Set the weight of the radio button.
radio3.LineFormat.Weight = 4;
 
//Set the line color of the radio button.
radio3.LineFormat.ForeColor = Color.Blue;
 
//Set the dash style of the radio button.
radio3.LineFormat.DashStyle = MsoLineDashStyle.Solid;
 
//Make the line format visible.
radio3.LineFormat.IsVisible = true;
 
//Make the fill format visible.
radio3.FillFormat.IsVisible = true;
 
//Get the shapes.
Aspose.Cells.Shape[] shapeobjects = new Aspose.Cells.Shape[] { box, radio1, radio2, radio3 };
 
//Group the shapes.
Aspose.Cells.GroupShape group = excelbook.Worksheets[0].Shapes.Group(shapeobjects);
 
//Save the excel file.
excelbook.Save("d:\\test\\groupshapes.xls");

[VB.NET]

'Instantiate a new Workbook.
Dim excelbook As Workbook = New Workbook()
 
'Add a group box to the first worksheet.
Dim box As Aspose.Cells.GroupBox = excelbook.Worksheets(0).Shapes.AddGroupBox(1, 0, 1, 0, 300, 250)
 
'Set the caption of the group box.
box.Text = "Age Groups"
box.Placement = PlacementType.FreeFloating
 
'Make it 2-D box.
box.Shadow = False
 
'Add a radio button.
Dim radio1 As Aspose.Cells.RadioButton = excelbook.Worksheets(0).Shapes.AddRadioButton(3, 0, 2, 0, 30, 110)
 
'Set its text string.
radio1.Text = "20-29"
 
'Set A1 cell as a linked cell for the radio button.
radio1.LinkedCell = "A1"
 
'Make the radio button 3-D.
radio1.Shadow = True
 
'Set the foreground color of the radio button.
radio1.FillFormat.ForeColor = Color.LightGreen
 
'Set the line style of the radio button.
radio1.LineFormat.Style = MsoLineStyle.ThickThin
 
'Set the weight of the radio button.
radio1.LineFormat.Weight = 4
 
'Set the line color of the radio button.
radio1.LineFormat.ForeColor = Color.Blue
 
'Set the dash style of the radio button.
radio1.LineFormat.DashStyle = MsoLineDashStyle.Solid
 
'Make the line format visible.
radio1.LineFormat.IsVisible = True
 
'Make the fill format visible.
radio1.FillFormat.IsVisible = True
 
'Add another radio button.
Dim radio2 As Aspose.Cells.RadioButton = excelbook.Worksheets(0).Shapes.AddRadioButton(6, 0, 2, 0, 30, 110)
 
'Set its text string.
radio2.Text = "30-39"
 
'Set A1 cell as a linked cell for the radio button.
radio2.LinkedCell = "A1"
 
'Make the radio button 3-D.
radio2.Shadow = True
 
'Set the foreground color of the radio button.
radio2.FillFormat.ForeColor = Color.LightGreen
 
'Set the line style of the radio button.
radio2.LineFormat.Style = MsoLineStyle.ThickThin
 
'Set the weight of the radio button.
radio2.LineFormat.Weight = 4
 
'Set the line color of the radio button.
radio2.LineFormat.ForeColor = Color.Blue
 
'Set the dash style of the radio button.
radio2.LineFormat.DashStyle = MsoLineDashStyle.Solid
 
'Make the line format visible.
radio2.LineFormat.IsVisible = True
 
'Make the fill format visible.
radio2.FillFormat.IsVisible = True
 
'Add another radio button.
Dim radio3 As Aspose.Cells.RadioButton = excelbook.Worksheets(0).Shapes.AddRadioButton(9, 0, 2, 0, 30, 110)
 
'Set its text string.
radio3.Text = "40-49"
 
'Set A1 cell as a linked cell for the radio button.
radio3.LinkedCell = "A1"
 
'Make the radio button 3-D.
radio3.Shadow = True
 
'Set the foreground color of the radio button.
radio3.FillFormat.ForeColor = Color.LightGreen
 
'Set the line style of the radio button.
radio3.LineFormat.Style = MsoLineStyle.ThickThin
 
'Set the weight of the radio button.
radio3.LineFormat.Weight = 4
 
'Set the line color of the radio button.
radio3.LineFormat.ForeColor = Color.Blue
 
'Set the dash style of the radio button.
radio3.LineFormat.DashStyle = MsoLineDashStyle.Solid
 
'Make the line format visible.
radio3.LineFormat.IsVisible = True
 
'Make the fill format visible.
radio3.FillFormat.IsVisible = True
 
'Get the shapes.
Dim shapeobjects() As Aspose.Cells.Shape = New Aspose.Cells.Shape() {box, radio1, radio2, radio3}
 
'Group the shapes.
Dim group As Aspose.Cells.GroupShape = excelbook.Worksheets(0).Shapes.Group(shapeobjects)
 
'Save the excel file.
excelbook.Save("d:\test\groupshapes.xls")
```

### See Also

* class [Shape](../shape)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
