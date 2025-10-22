##Class DxfCollection
Aspose.Cells.DxfCollection class. Represents the master differential formatting records
## DxfCollection class
Represents the master differential formatting records.
```csharp
public class DxfCollection : CollectionBase<Style>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/dxfcollection/item/) { get; } | Gets the element at the specified index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Style) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Style, IComparer&lt;Style&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Style, IComparer&lt;Style&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Style) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Style[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Style[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Style[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Style&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Style&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Style&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Style&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsClassDxfCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the DxfCollection from the workbook
DxfCollection dxfCollection = workbook.Worksheets.Dxfs;
// Create and add styles to the workbook (they will be available in DxfCollection)
Style headerStyle = workbook.CreateStyle();
headerStyle.Font.Name = "Calibri";
headerStyle.Font.Size = 14;
headerStyle.Font.IsBold = true;
headerStyle.ForegroundColor = System.Drawing.Color.LightGray;
headerStyle.Pattern = BackgroundType.Solid;
Style dataStyle = workbook.CreateStyle();
dataStyle.Font.Name = "Calibri";
dataStyle.Font.Size = 11;
dataStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
dataStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
// Access styles through DxfCollection
Console.WriteLine("Number of styles in DxfCollection: " + dxfCollection.Count);
Console.WriteLine("First style font: " + dxfCollection[0].Font.Name);
// Apply styles to cells
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A1"].SetStyle(dxfCollection[0]);
worksheet.Cells["A2"].PutValue("Data");
worksheet.Cells["A2"].SetStyle(dxfCollection[1]);
// Modify a style through DxfCollection
dxfCollection[1].Font.Color = System.Drawing.Color.Blue;
worksheet.Cells["A3"].PutValue("Modified Data");
worksheet.Cells["A3"].SetStyle(dxfCollection[1]);
// Save the result
workbook.Save("CellsClassDxfCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Style](../style/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
