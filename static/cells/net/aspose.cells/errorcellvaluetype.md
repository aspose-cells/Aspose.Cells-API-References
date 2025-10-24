##Enum ErrorCellValueType
Aspose.Cells.ErrorCellValueType enum. Represents a cell value which contains an error
## ErrorCellValueType enumeration
Represents a cell value which contains an error.
```csharp
public enum ErrorCellValueType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Blocked | `10` | Represents the value of a cell containing a #BLOCKED! error. |
| Busy | `14` | Represents the value of a cell containing a #BUSY! error. |
| Calc | `13` | Represents the value of a cell containing a #CALC! error. |
| Connect | `9` | Represents the value of a cell containing a #CONNECT! error. |
| Name | `4` | Represents the value of a cell containing a #NAME? error. |
| Field | `12` | Represents the value of a cell containing a #FIELD! error. |
| Spill | `8` | Represents the value of a cell containing a #SPILL! error. |
| Unknown | `11` | Represents the value of a cell containing a #UNKNOWN! error. |
| TimeOut | `19` | Represents the value of a cell containing a #TIMEOUT! error. |
| External | `18` | Represents the value of a cell containing an #EXTERNAL! error. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassErrorCellValueTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set a formula that will result in a spill error
worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
try
{
// Calculate formulas to trigger the error
workbook.CalculateFormula();
}
catch (Exception)
{
// Expected spill error
}
// Get the cell's rich value
CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
// Check the error type
if (richValue.ErrorValue == ErrorCellValueType.Spill)
{
Console.WriteLine("Cell contains a spill error as expected");
}
// Save the workbook
workbook.Save("ErrorCellValueTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
