##RadioButton.GetOptionIndex
RadioButton method. Gets the option index onebased in all the radio buttons of the GroupBox which contains this radio button
## RadioButton.GetOptionIndex method
Gets the option index (one-based) in all the radio buttons of the GroupBox which contains this radio button.
```csharp
public int GetOptionIndex()
```
### Remarks
If this radio button is not in the GroupBox, returns the option index in all radio buttons that are not in any GroupBox
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class RadioButtonMethodGetOptionIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a group box to contain radio buttons
GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
// Add three radio buttons to the group box
RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);
// Set the radio buttons to be part of the group box
radioButton1.Placement = PlacementType.FreeFloating;
radioButton2.Placement = PlacementType.FreeFloating;
radioButton3.Placement = PlacementType.FreeFloating;
try
{
// Get the option index for each radio button
int index1 = radioButton1.GetOptionIndex();
int index2 = radioButton2.GetOptionIndex();
int index3 = radioButton3.GetOptionIndex();
Console.WriteLine($"RadioButton1 Option Index: {index1}");
Console.WriteLine($"RadioButton2 Option Index: {index2}");
Console.WriteLine($"RadioButton3 Option Index: {index3}");
// Check the first radio button to demonstrate selection
radioButton1.IsChecked = true;
Console.WriteLine("RadioButton1 is checked");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
}
// Save the result
workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
}
}
}
```
### See Also
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
