##Enum CellValueType
Aspose.Cells.CellValueType enum. Specifies a cell value type
## CellValueType enumeration
Specifies a cell value type.
```csharp
public enum CellValueType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| IsUnknown | `0` | Cell value type is unknown. |
| IsNull | `1` | Blank cell. Corresponding value should be null. |
| IsNumeric | `2` | Cell value is numeric. Corresponding value must be int or double. |
| IsDateTime | `4` | Cell value is datetime. Corresponding value must be DateTime. |
| IsString | `8` | Cell value is string. Corresponding value must be string. |
| IsBool | `16` | Cell value is boolean. Corresponding value must be bool. |
| IsError | `32` | Cell contains error value. Corresponding value must be error string. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellValueTypeDemo
{
public static void CellValueTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue(123); // Numeric value
worksheet.Cells["A2"].PutValue("Hello World"); // String value
worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
worksheet.Cells["A4"].PutValue(true); // Boolean value
worksheet.Cells["A5"].PutValue(null); // Null value
// Check and display the value types of the cells
DisplayCellValueType(worksheet.Cells["A1"]);
DisplayCellValueType(worksheet.Cells["A2"]);
DisplayCellValueType(worksheet.Cells["A3"]);
DisplayCellValueType(worksheet.Cells["A4"]);
DisplayCellValueType(worksheet.Cells["A5"]);
// Save the workbook
workbook.Save("CellValueTypeExample.xlsx");
workbook.Save("CellValueTypeExample.pdf");
}
private static void DisplayCellValueType(Cell cell)
{
Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");
switch (cell.Type)
{
case CellValueType.IsNumeric:
Console.WriteLine("The cell contains a numeric value.");
break;
case CellValueType.IsString:
Console.WriteLine("The cell contains a string value.");
break;
case CellValueType.IsDateTime:
Console.WriteLine("The cell contains a DateTime value.");
break;
case CellValueType.IsBool:
Console.WriteLine("The cell contains a boolean value.");
break;
case CellValueType.IsNull:
Console.WriteLine("The cell is blank.");
break;
case CellValueType.IsError:
Console.WriteLine("The cell contains an error value.");
break;
default:
Console.WriteLine("The cell value type is unknown.");
break;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
