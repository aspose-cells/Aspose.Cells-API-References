##Class RowCollection
Aspose.Cells.RowCollection class. Collects the Row objects that represent the individual rows in a worksheet
## RowCollection class
Collects the [`Row`](../row/) objects that represent the individual rows in a worksheet.
```csharp
public class RowCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Gets the number of rows in this collection. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Gets a [`Row`](../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before. |
## Methods
| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Clear all rows and cells. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Gets an enumerator that iterates rows through this collection |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Gets an enumerator that iterates rows through this collection |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Gets the row object by the position in the list. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Remove the row item at the specified index(position) in this collection. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class RowCollectionDemo
{
public static void RowCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
worksheet.Cells["A3"].PutValue("Aspose.Cells");
// Get the Rows collection
RowCollection rows = worksheet.Cells.Rows;
// Get the number of rows in the collection
int rowCount = rows.Count;
Console.WriteLine("Number of rows: " + rowCount);
// Get the first row
Row firstRow = rows[0];
Console.WriteLine("First row index: " + firstRow.Index);
// Iterate through the rows using GetEnumerator
IEnumerator enumerator = rows.GetEnumerator();
while (enumerator.MoveNext())
{
Row row = (Row)enumerator.Current;
Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
}
// Get a row by index
Row specificRow = rows.GetRowByIndex(1);
Console.WriteLine("Specific row index: " + specificRow.Index);
// Clear all rows and cells
rows.Clear();
Console.WriteLine("Rows cleared.");
// Save the workbook
workbook.Save("RowCollectionExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
