##Enum CheckValueType
Aspose.Cells.Drawing.CheckValueType enum. Represents the check value type of the check box
## CheckValueType enumeration
Represents the check value type of the check box.
```csharp
public enum CheckValueType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| UnChecked | `0` | UnChecked |
| Checked | `1` | Checked |
| Mixed | `2` | Mixed |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassCheckValueTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add checkboxes to the worksheet
int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);
// Get the checkboxes and set their properties
Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];
// Set checkbox values and checked state
checkbox1.Value = true;
checkbox1.CheckedValue = CheckValueType.Checked;
checkbox2.Value = false;
checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked
// Link checkboxes to cells
checkbox1.LinkedCell = "A1";
checkbox2.LinkedCell = "A2";
// Output the cell values to demonstrate the link
Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
