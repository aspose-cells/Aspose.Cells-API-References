##CheckBox.Shadow
CheckBox property. Indicates whether the combobox has 3D shading
## CheckBox.Shadow property
Indicates whether the combobox has 3-D shading.
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
public class CheckBoxPropertyShadowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a checkbox to the worksheet and get its index
int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
// Configure checkbox properties
checkBox.Text = "Enable Feature";
checkBox.Value = true;
// Demonstrate Shadow property
checkBox.Shadow = true; // Enable shadow effect
workbook.Save("CheckBoxWithShadow.xlsx");
checkBox.Shadow = false; // Disable shadow effect
workbook.Save("CheckBoxWithoutShadow.xlsx");
}
}
}
```
### See Also
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
