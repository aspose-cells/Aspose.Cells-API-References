##Column.GroupLevel
Column property. Gets the group level of the column
## Column.GroupLevel property
Gets the group level of the column.
```csharp
public byte GroupLevel { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnPropertyGroupLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Group columns (isHidden parameter set to false)
worksheet.Cells.GroupColumns(0, 2, false);
// Get the group level of the first column
int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
// Output the group level
Console.WriteLine("Group level of first column: " + groupLevel);
// Save the workbook
workbook.Save("GroupLevelDemo.xlsx");
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
