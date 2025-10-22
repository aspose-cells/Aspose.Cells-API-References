##ListColumnCollection.Item
ListColumnCollection property. Gets the ListColumn by the index
## ListColumnCollection indexer (1 of 2)
Gets the ListColumn by the index.
```csharp
public ListColumn this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
the ListColumn object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("T1");
worksheet.Cells["B1"].PutValue("T2");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(2);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
ListObject listObj = worksheet.ListObjects[index];
// Access list columns using Item property
ListColumn firstColumn = listObj.ListColumns[0];
Console.WriteLine("First column name: " + firstColumn.Name);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## ListColumnCollection indexer (2 of 2)
Gets the ListColumn by the name.
```csharp
public ListColumn this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the ListColumn |
### Return Value
The ListColumn object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class ListColumnCollectionPropertyItemDemo2
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Price";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 2.5;
worksheet.Cells["A3"].Value = "Banana";
worksheet.Cells["B3"].Value = 1.8;
int tableIndex = worksheet.ListObjects.Add("A1", "B3", true); // Split range into start/end cells
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowHeaderRow = true;
ListColumnCollection listColumns = table.ListColumns;
ListColumn column = listColumns["Product"];
Console.WriteLine("Current column name: " + column.Name);
column.Name = "Item";
Console.WriteLine("Updated column name: " + column.Name);
workbook.Save("ListColumnCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
