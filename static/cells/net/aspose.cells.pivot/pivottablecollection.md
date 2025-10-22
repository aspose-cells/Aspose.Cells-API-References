##Class PivotTableCollection
Aspose.Cells.Pivot.PivotTableCollection class. Represents the collection of all the PivotTable objects on the specified worksheet
## PivotTableCollection class
Represents the collection of all the PivotTable objects on the specified worksheet.
```csharp
public class PivotTableCollection : CollectionBase<PivotTable>, IDisposable
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottablecollection/item/) { get; } | Gets the PivotTable report by index. (3 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_1)(PivotTable, string, string) | Adds a new PivotTable based on another PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_5)(string, string, string) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add)(PivotTable, int, int, string) | Adds a new PivotTable based on another PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_2)(string, int, int, string) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_6)(string, string, string, bool) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_3)(string, int, int, string, bool) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_7)(string, string, string, bool, bool) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_9)(string[], bool, PivotPageFields, string, string) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_4)(string, int, int, string, bool, bool) | Adds a new PivotTable. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add/#add_8)(string[], bool, PivotPageFields, int, int, string) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivottablecollection/clear/#clear)() | Clear all pivot tables. (2 methods) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotTable) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotTable[], int, int) |  |
| [Dispose](../../aspose.cells.pivot/pivottablecollection/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTable) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTable, int, int) |  |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove/#remove)(PivotTable) | Deletes the specified PivotTable and delete the PivotTable data |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove/#remove_1)(PivotTable, bool) | Deletes the specified PivotTable |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat/#removeat)(int) | Deletes the PivotTable at the specified index and delete the PivotTable data (2 methods) |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat/#removeat_2)(int, bool) | Deletes the PivotTable at the specified index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Drawing;
public class PivotTableCollectionDemo
{
public static void PivotTableCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add sample data to the worksheet
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";
cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;
cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;
// Access the PivotTableCollection
PivotTableCollection pivots = sheet.PivotTables;
// Add a PivotTable to the worksheet
int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
// Configure the PivotTable
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
// Set PivotTable style
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Change PivotField's attributes
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";
// Add PivotFilter
int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[filterIndex];
filter.AutoFilter.FilterTop10(0, false, false, 2);
// Add PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;
// Refresh and calculate the PivotTable data
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
workbook.Save("PivotTableCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotTable](../pivottable/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
