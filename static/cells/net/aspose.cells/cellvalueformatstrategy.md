##Enum CellValueFormatStrategy
Aspose.Cells.CellValueFormatStrategy enum. Specifies how to apply style for the value of the cell
## CellValueFormatStrategy enumeration
Specifies how to apply style for the value of the cell.
```csharp
public enum CellValueFormatStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Not formatted. |
| CellStyle | `1` | Only formatted with the cell's original style. |
| DisplayStyle | `2` | Formatted with the cell's displayed style. |
| DisplayString | `3` | Gets the displayed string shown in ms excel. The main difference from DisplayStyle is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellValueFormatStrategyDemo
{
public static void CellValueFormatStrategyExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(DateTime.Now);
worksheet.Cells["B1"].PutValue("Number");
worksheet.Cells["B2"].PutValue(12345.6789);
worksheet.Cells["C1"].PutValue("Text");
worksheet.Cells["C2"].PutValue("Hello World");
// Apply different CellValueFormatStrategy to demonstrate their effects
// None: Not formatted
string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
Console.WriteLine($"None: {valueNone}");
// CellStyle: Only formatted with the cell's original style
string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
Console.WriteLine($"CellStyle: {valueCellStyle}");
// DisplayStyle: Formatted with the cell's displayed style
string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");
// DisplayString: Gets the displayed string shown in MS Excel
string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
Console.WriteLine($"DisplayString: {valueDisplayString}");
// Save the workbook to a file
workbook.Save("CellValueFormatStrategyExample.xlsx");
workbook.Save("CellValueFormatStrategyExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
