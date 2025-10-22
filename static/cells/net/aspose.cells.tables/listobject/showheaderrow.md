##ListObject.ShowHeaderRow
ListObject property. Gets and sets whether this ListObject show header row
## ListObject.ShowHeaderRow property
Gets and sets whether this ListObject show header row.
```csharp
public bool ShowHeaderRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyShowHeaderRowDemo
{
public static void Run()
{
// Create a workbook and worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
// Create a list object/table
int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.TableStyleType = TableStyleType.TableStyleMedium2;
table.ShowHeaderRow = true; // Header row is visible by default
Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);
// Hide the header row
table.ShowHeaderRow = false;
Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);
// Save the workbook
workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
