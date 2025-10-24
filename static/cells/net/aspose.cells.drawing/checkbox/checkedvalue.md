##CheckBox.CheckedValue
CheckBox property. Gets or set checkbox value
## CheckBox.CheckedValue property
Gets or set checkbox' value.
```csharp
public CheckValueType CheckedValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CheckBoxPropertyCheckedValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a checkbox to the worksheet
CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);
// Set the checkbox value to Checked
checkBox.CheckedValue = CheckValueType.Checked;
// Save the workbook
workbook.Save("CheckBoxCheckedValueDemo.xlsx");
// Load the saved workbook to verify
Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
// Output the checkbox state
Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
}
}
}
```
### See Also
* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
