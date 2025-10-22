##Class PivotTableFormatCollection
Aspose.Cells.Pivot.PivotTableFormatCollection class. Represents the collection of formats applied to PivotTable
## PivotTableFormatCollection class
Represents the collection of formats applied to PivotTable.
```csharp
public class PivotTableFormatCollection : CollectionBase<PivotTableFormat>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottableformatcollection/item/) { get; } | Gets the format by the index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottableformatcollection/add/)() | Add a [`PivotTableFormat`](../pivottableformat/). |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotTableFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotTableFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FormatArea](../../aspose.cells.pivot/pivottableformatcollection/formatarea/)(PivotFieldType, int, PivotFieldSubtotalType, PivotTableSelectionType, bool, bool, Style) | Formats selected area. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Drawing;
public class PivotTableFormatCollectionDemo
{
public static void PivotTableFormatCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[2, 1].Value = 2020;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 0].Value = "Apple";
worksheet.Cells[3, 1].Value = 2021;
worksheet.Cells[3, 2].Value = 70;
worksheet.Cells[4, 0].Value = "Banana";
worksheet.Cells[4, 1].Value = 2021;
worksheet.Cells[4, 2].Value = 80;
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Access the PivotTableFormatCollection
PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;
// Add a format to the collection
int formatIndex = formatCollection.Add();
PivotTableFormat pivotFormat = formatCollection[formatIndex];
// Define the format area
PivotTableFormat newFormat = formatCollection.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, new Style());
// Set the style for the format
Style style = new Style();
style.BackgroundColor = Color.LightBlue;
newFormat.SetStyle(style);
// Save the workbook
workbook.Save("PivotTableFormatCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotTableFormat](../pivottableformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
