##RadioButton.GroupBox
RadioButton property. Gets the GroupBox that contains this RadioButton
## RadioButton.GroupBox property
Gets the GroupBox that contains this RadioButton.
```csharp
public GroupBox GroupBox { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class RadioButtonPropertyGroupBoxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a group box to contain radio buttons
GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
groupBox.Name = "OptionsGroup";
groupBox.Shadow = true;
// Add radio buttons to the worksheet (not yet in group box)
RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
// Display initial GroupBox property values (should be null)
Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));
// Add radio buttons to the group box by setting placement
radioButton1.Placement = PlacementType.FreeFloating;
radioButton2.Placement = PlacementType.FreeFloating;
// Move radio buttons inside the group box
radioButton1.Top = groupBox.Top + 20;
radioButton1.Left = groupBox.Left + 20;
radioButton2.Top = groupBox.Top + 50;
radioButton2.Left = groupBox.Left + 20;
// Display GroupBox property values after grouping
Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);
// Demonstrate group behavior
radioButton1.IsChecked = true;
Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);
// Save the result
workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
}
}
}
```
### See Also
* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
