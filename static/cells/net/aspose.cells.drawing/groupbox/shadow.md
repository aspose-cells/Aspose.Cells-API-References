##GroupBox.Shadow
GroupBox property. Indicates whether the groupbox has shadow
## GroupBox.Shadow property
Indicates whether the groupbox has shadow.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class GroupBoxPropertyShadowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a group box with shadow
GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
groupBoxWithShadow.Shadow = true;
groupBoxWithShadow.Text = "GroupBox with Shadow";
// Add a group box without shadow
GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
groupBoxWithoutShadow.Shadow = false;
groupBoxWithoutShadow.Text = "GroupBox without Shadow";
// Add radio buttons inside the group boxes to demonstrate grouping
RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
radio1.Text = "Option 1";
radio1.LinkedCell = "A1";
RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
radio2.Text = "Option 2";
radio2.LinkedCell = "A1";
// Group the shapes
Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
worksheet.Shapes.Group(shapes);
// Save the workbook
workbook.Save("GroupBoxShadowDemo.xlsx");
}
}
}
```
### See Also
* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
