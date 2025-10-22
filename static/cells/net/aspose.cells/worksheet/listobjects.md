##Worksheet.ListObjects
Worksheet property. Gets all ListObjects in this worksheet
## Worksheet.ListObjects property
Gets all ListObjects in this worksheet.
```csharp
public ListObjectCollection ListObjects { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class WorksheetPropertyListObjectsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(200);
// Create a ListObject (table)
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
table.DisplayName = "ProductTable";
table.ShowTotals = true;
// Resize the table to include more rows
table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
// Add more data to the extended table
worksheet.Cells["A4"].PutValue("Item3");
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["A5"].PutValue("Item4");
worksheet.Cells["B5"].PutValue(400);
// Access the table through ListObjects property
ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
retrievedTable.ShowHeaderRow = true;
// Save the workbook
workbook.Save("ListObjectsDemo.xlsx");
}
}
}
```
### See Also
* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
