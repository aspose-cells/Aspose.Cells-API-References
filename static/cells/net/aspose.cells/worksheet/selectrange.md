##Worksheet.SelectRange
Worksheet method. Selects a range
## Worksheet.SelectRange method
Selects a range.
```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns,
bool removeOthers)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| totalRows | Int32 | The number of rows. |
| totalColumns | Int32 | The number of columns |
| removeOthers | Boolean | True means removing other selected range and only select this range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Select range from row 1, column 1 to row 5, column 5 (B2:F6) and make it active
worksheet.SelectRange(1, 1, 5, 5, true);
Console.WriteLine("Active cell: " + worksheet.ActiveCell);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
