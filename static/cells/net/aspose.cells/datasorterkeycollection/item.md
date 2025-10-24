##DataSorterKeyCollection.Item
DataSorterKeyCollection property. Gets and sets DataSorterKey by index
## DataSorterKeyCollection indexer
Gets and sets [`DataSorterKey`](../../datasorterkey/) by index.
```csharp
public DataSorterKey this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class DataSorterKeyCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["A4"].PutValue("Bob");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["B3"].PutValue(92);
worksheet.Cells["B4"].PutValue(78);
// Create a list object (table)
int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = worksheet.ListObjects[index];
// Add sort key (sort by Score column in descending order)
table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
table.AutoFilter.Sorter.Sort();
// Demonstrate Item property usage
DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
