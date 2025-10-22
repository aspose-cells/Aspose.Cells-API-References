##Cells.IsBlankColumn
Cells method. Checks whether given column is blankdoes not contain any data
## Cells.IsBlankColumn method
Checks whether given column is blank(does not contain any data).
```csharp
public bool IsBlankColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | the column index |
### Return Value
true if given column does not contain any data
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodIsBlankColumnWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Check if column 2 is blank (should be true for new worksheet)
Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));
// Add data to column 2
worksheet.Cells["B1"].PutValue("Test Data");
// Check again (should now be false)
Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));
// Create another worksheet with completely blank columns
Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");
// Check a column in the blank worksheet (should be true)
Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
