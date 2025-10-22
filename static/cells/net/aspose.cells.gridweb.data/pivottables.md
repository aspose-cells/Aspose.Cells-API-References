##Class PivotTables
Aspose.Cells.GridWeb.Data.PivotTables class. Represents a collection of all the PivotTable objects
## PivotTables class
Represents a collection of all the [`PivotTable`](../pivottable/) objects
```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Gets the number of elements contained in the PivotTables instance |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Gets a value indicating whether access to the PivotTables is synchronized (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Gets a PivotTable object by index. (2 indexers) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Gets the parent object for the specified object. Read-only. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Gets an object that can be used to synchronize access to the PivotTables. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Adds a PivotTable object from the specified PivotCache to a new worksheet |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Adds a PivotTable object from the specified PivotCache to a new worksheet |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Adds a PivotTable object from the specified PivotCache to the specified worksheet |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Adds a PivotTable object from the specified PivotCache to the specified worksheet |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Removes all PivotTable objects and all PivotCache objects in the control. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Returns true if exists pivottable name tableName. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Copies the entire PivotTable to a compatible one-dimensional Array, starting at the specified index of the target array |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Returns an IEnumerator for the PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | ReDataBinds data source to the PivotTable report. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | ReDataBinds data source to all PivotTable report. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Removes the specified PivotTable object from the PivotTables and the related PivotCache if it is not used by other PivotTable |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Removes the specified PivotTable object from the PivotTables and the related PivotCache if it is not used by other PivotTable |
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
