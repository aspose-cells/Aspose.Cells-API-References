##Class TableStyleCollection
Aspose.Cells.Tables.TableStyleCollection class. Represents all custom table styles
## TableStyleCollection class
Represents all custom table styles.
```csharp
public class TableStyleCollection : CollectionBase<TableStyle>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DefaultPivotStyleName](../../aspose.cells.tables/tablestylecollection/defaultpivotstylename/) { get; set; } | Gets and sets the default style name of pivot table . |
| [DefaultTableStyleName](../../aspose.cells.tables/tablestylecollection/defaulttablestylename/) { get; set; } | Gets and sets the default style name of the table. |
| [Item](../../aspose.cells.tables/tablestylecollection/item/) { get; } | Gets the table style by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [AddPivotTableStyle](../../aspose.cells.tables/tablestylecollection/addpivottablestyle/)(string) | Adds a custom pivot table style. |
| [AddTableStyle](../../aspose.cells.tables/tablestylecollection/addtablestyle/)(string) | Adds a custom table style. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyle) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyle[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyle&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyle&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [GetBuiltinTableStyle](../../aspose.cells.tables/tablestylecollection/getbuiltintablestyle/)(TableStyleType) | Gets the builtin table style |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TablesClassTableStyleCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the table style collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Display default style names
Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
// Change the default table style
tableStyles.DefaultTableStyleName = "TableStyleMedium9";
// Save the workbook
workbook.Save("TableStylesDemo.xlsx");
// Verify the change by loading the saved file
Workbook verifyWorkbook = new Workbook("TableStylesDemo.xlsx");
Console.WriteLine("New Default Table Style: " +
verifyWorkbook.Worksheets.TableStyles.DefaultTableStyleName);
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyle](../tablestyle/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
