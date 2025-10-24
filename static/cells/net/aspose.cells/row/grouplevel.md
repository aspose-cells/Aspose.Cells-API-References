##Row.GroupLevel
Row property. Gets the group level of the row
## Row.GroupLevel property
Gets the group level of the row.
```csharp
public byte GroupLevel { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyGroupLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Group rows 4-6 (hidden = false)
worksheet.Cells.GroupRows(3, 5, false);
// Access the group level of row 4
int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
Console.WriteLine("Group level of row 4: " + groupLevel);
// Ungroup the rows
worksheet.Cells.UngroupRows(3, 5);
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
