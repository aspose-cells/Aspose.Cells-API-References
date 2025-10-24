##Class CellWatch
Aspose.Cells.CellWatch class. Represents Cell Watch Item in the watch window
## CellWatch class
Represents Cell Watch Item in the 'watch window'.
```csharp
public class CellWatch
```
## Constructors
| Name | Description |
| --- | --- |
| [CellWatch](cellwatch/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Gets and sets the name of the cell. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Gets and sets the column of the cell. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Gets and sets the row of the cell. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellWatchDemo
{
public static void CellWatchExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet.
Worksheet sheet = workbook.Worksheets[0];
// Add Cell Watch Item into the watch window
int watchIndex = sheet.CellWatches.Add("B2");
// Retrieve the CellWatch object
CellWatch cellWatch = sheet.CellWatches[watchIndex];
// Setting properties
cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
cellWatch.CellName = "B2";
// Save the workbook
workbook.Save("CellWatchExample.xlsx");
workbook.Save("CellWatchExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
