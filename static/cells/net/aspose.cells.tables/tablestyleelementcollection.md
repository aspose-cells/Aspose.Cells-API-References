##Class TableStyleElementCollection
Aspose.Cells.Tables.TableStyleElementCollection class. Represents all elements of the table style
## TableStyleElementCollection class
Represents all elements of the table style.
```csharp
public class TableStyleElementCollection : CollectionBase<TableStyleElement>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/tablestyleelementcollection/item/) { get; } | Gets an element of the table style by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.tables/tablestyleelementcollection/add/)(TableStyleElementType) | Adds an element. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyleElement) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyleElement[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyleElement&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleElementCollectionDemo
{
public static void TableStyleElementCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create styles for the first and last columns
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;
Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.Pattern = BackgroundType.Solid;
lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;
// Define a custom table style name
string tableStyleName = "Custom1";
// Access the table styles collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Add a new table style to the collection
int index1 = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles[index1];
// Access the table style elements collection
TableStyleElementCollection elements = tableStyle.TableStyleElements;
// Add and configure the first column style element
index1 = elements.Add(TableStyleElementType.FirstColumn);
TableStyleElement element = elements[index1];
element.SetElementStyle(firstColumnStyle);
// Add and configure the last column style element
index1 = elements.Add(TableStyleElementType.LastColumn);
element = elements[index1];
element.SetElementStyle(lastColumnStyle);
// Populate the worksheet with sample data
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 5; column++)
{
cells[row, column].PutValue(row * column);
}
}
// Add a table to the worksheet
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
// Apply the custom table style to the table
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
table.TableStyleName = tableStyleName;
// Save the workbook
workbook.Save("TableStyleElementCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyleElement](../tablestyleelement/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
