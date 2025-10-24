##Class SlicerCacheItemCollection
Aspose.Cells.Slicers.SlicerCacheItemCollection class. Represent the collection of SlicerCacheItem
## SlicerCacheItemCollection class
Represent the collection of SlicerCacheItem
```csharp
public class SlicerCacheItemCollection : CollectionBase<SlicerCacheItem>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.slicers/slicercacheitemcollection/count/) { get; } | Gets the count of the SlicerCacheItem. |
| [Item](../../aspose.cells.slicers/slicercacheitemcollection/item/) { get; } | Gets the SlicerCacheItem object by index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SlicerCacheItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SlicerCacheItem, IComparer&lt;SlicerCacheItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SlicerCacheItem, IComparer&lt;SlicerCacheItem&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SlicerCacheItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SlicerCacheItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SlicerCacheItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SlicerCacheItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SlicerCacheItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SlicerCacheItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SlicerCacheItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SlicerCacheItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SlicerCacheItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SlicerCacheItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicersClassSlicerCacheItemCollectionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Set up sample data
cells["A1"].Value = "fruit";
cells["A2"].Value = "grape";
cells["A3"].Value = "blueberry";
cells["A4"].Value = "kiwi";
cells["A5"].Value = "cherry";
cells["A6"].Value = "grape";
cells["A7"].Value = "blueberry";
cells["A8"].Value = "kiwi";
cells["A9"].Value = "cherry";
cells["B1"].Value = "year";
cells["B2"].Value = 2020;
cells["B3"].Value = 2020;
cells["B4"].Value = 2020;
cells["B5"].Value = 2020;
cells["B6"].Value = 2021;
cells["B7"].Value = 2021;
cells["B8"].Value = 2021;
cells["B9"].Value = 2021;
cells["C1"].Value = "amount";
cells["C2"].Value = 50;
cells["C3"].Value = 60;
cells["C4"].Value = 70;
cells["C5"].Value = 80;
cells["C6"].Value = 90;
cells["C7"].Value = 100;
cells["C8"].Value = 110;
cells["C9"].Value = 120;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
// Add slicer
int slicerIndex = sheet.Slicers.Add(pivot, "E12", "fruit");
Slicer slicer = sheet.Slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
// Demonstrate SlicerCacheItemCollection usage
SlicerCacheItemCollection cacheItems = slicer.SlicerCache.SlicerCacheItems;
Console.WriteLine("Slicer Items Count: " + cacheItems.Count);
foreach (SlicerCacheItem item in cacheItems)
{
Console.WriteLine("Item: " + item.Value + ", Selected: " + item.Selected);
}
workbook.Save("SlicerCacheItemCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SlicerCacheItem](../slicercacheitem/)
* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)
