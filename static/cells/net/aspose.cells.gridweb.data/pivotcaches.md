##Class PivotCaches
Aspose.Cells.GridWeb.Data.PivotCaches class. Represents the collection of memory caches from the PivotTable reports in a workbook. Each memory cache is represented by a PivotCache object
## PivotCaches class
Represents the collection of memory caches from the PivotTable reports in a workbook. Each memory cache is represented by a [`PivotCache`](../pivotcache/) object.
```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Gets the number of elements contained in the PivotCaches instance |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Gets a value indicating whether access to the PivotCaches is synchronized (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Gets PivotCache object by index. (2 indexers) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Gets the parent object for the specified object. Read-only. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Gets an object that can be used to synchronize access to the PivotCaches. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Adds a PivotCache from DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Adds a PivotCache from DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Adds a PivotCahe from DataTable using the specified name. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Adds a PivotCahe from DataView using the specified name. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Adds a PivotCache from sheet |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Adds a PivotCache from sheet using the specified name. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Removes all PivotCache objects and all PivotTable objects in the control. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Copies the entire PivotCache to a compatible one-dimensional Array, starting at the specified index of the target array |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Returns an IEnumerator for the PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Returns the index of the specified PivotCache in the collection |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Removes the specified PivotCache object from the PivotCaches and the related PivotTable using the pivotCache as data source. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Removes the specified PivotCache object from the PivotCaches and the related PivotTable using the pivotCache as data source. |
### Remarks
NOTE: This class is now obsolete. please use GridPivotTableCollection Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
[C#]
//On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
sourceRange.StartRow = 0;
sourceRange.StartColumn = 0;
sourceRange.EndRow = 10;
sourceRange.EndColumn = 5;
PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);
PivotTable table = cache.CreatePivotTable();
table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
table.PivotFields[3].Function = PivotFieldFunction.Count;
table.PivotFields[5].Function = PivotFieldFunction.Sum;
table.DataBind();
//Creates a PivotTable report from DataView or DataTable.
DataView dataView;//Or  DataTable dataTable;
.
.
.
Sets dataView(dataTable) Value
.
.
.
PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
//Or PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
PivotTable table = cache.CreatePivotTable();
table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
table.DataBind();
[VB]
'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
sourceRange.StartRow = 0
sourceRange.StartColumn = 0
sourceRange.EndRow = 10
sourceRange.EndColumn = 5
Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)
Dim table As PivotTable =  cache.CreatePivotTable()
table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
table.PivotFields(3).Function = PivotFieldFunction.Count
table.PivotFields(5).Function = PivotFieldFunction.Sum
table.DataBind()
'Creates a PivotTable report from DataView or DataTable.
Dim dataView As DataView ' Or Dim dataTable As DataTable
.
.
Sets dataView(dataTable) Value
.
.
.
Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
Dim table As PivotTable =  cache.CreatePivotTable()
table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
table.DataBind()
```
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
