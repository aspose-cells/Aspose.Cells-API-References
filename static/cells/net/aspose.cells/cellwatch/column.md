##CellWatch.Column
CellWatch property. Gets and sets the column of the cell
## CellWatch.Column property
Gets and sets the column of the cell.
```csharp
public int Column { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellWatchPropertyColumnDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int watchIndex = sheet.CellWatches.Add("B2");
CellWatch cellWatch = sheet.CellWatches[watchIndex];
Console.WriteLine("Initial Column: " + cellWatch.Column);
cellWatch.Column = 1;
Console.WriteLine("Modified Column: " + cellWatch.Column);
workbook.Save("CellWatchColumnDemo.xlsx");
}
}
}
```
### See Also
* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
