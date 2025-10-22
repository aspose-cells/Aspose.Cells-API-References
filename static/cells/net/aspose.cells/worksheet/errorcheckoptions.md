##Worksheet.ErrorCheckOptions
Worksheet property. Gets error check setting applied on certain ranges
## Worksheet.ErrorCheckOptions property
Gets error check setting applied on certain ranges.
```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyErrorCheckOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Enable error checking options
ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
ErrorCheckOption option = options[0]; // Properly access first option using indexer
option.SetErrorCheck(ErrorCheckType.TextDate, true);
option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
// Get count of ranges for the option
int rangeCount = option.GetCountOfRange();
Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
// Save the workbook
workbook.Save("ErrorCheckOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
