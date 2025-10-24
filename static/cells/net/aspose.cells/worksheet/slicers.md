##Worksheet.Slicers
Worksheet property. Get the Slicer collection in the worksheet
## Worksheet.Slicers property
Get the Slicer collection in the worksheet
```csharp
public SlicerCollection Slicers { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class WorksheetPropertySlicersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for the table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(30);
// Add a table
int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
// Add slicers to the worksheet
worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
worksheet.Slicers.Add(table, 1, "D1");
worksheet.Slicers.Add(table, table.ListColumns[0], "G1");
// Save the workbook
workbook.Save("SlicersDemo.xlsx");
}
}
}
```
### See Also
* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
