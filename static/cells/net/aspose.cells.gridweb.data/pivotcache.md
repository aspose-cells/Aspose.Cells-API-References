##Class PivotCache
Aspose.Cells.GridWeb.Data.PivotCache class. Represents the memory cache for a PivotTable report. The PivotCache object is a member of the PivotCaches collection
## PivotCache class
Represents the memory cache for a PivotTable report. The PivotCache object is a member of the [`PivotCaches`](../pivotcaches/) collection.
```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```
## Properties
| Name | Description |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Returns the data source of System.Data.DataTable for the PivotTable report. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Returns the data source of System.Data.DataView for the PivotTable report. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Returns the index of this object in Parent |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Returns the name of PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Returns the parent object for the specified object(the container of PivotCache). Read-only. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Returns the range of the data source using with SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Returns the data source of WebWorksheet for the PivotTable report. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Represents the type of the source data |
## Methods
| Name | Description |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Creates PivotTable report to a new Sheet. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Creates PivotTable report to a new Sheet. The name of the pivotTable object |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Creates PivotTable report to the targetSheet. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Creates PivotTable report to the targetSheet. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Determines whether two Object instances are equal. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Serves as a hash function for a particular type, suitable for use in hashing algorithms and data structures like a hash table. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Resets the source data |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Resets the source data |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Resets the source data |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Returns a String that represents the current Object |
### Remarks
NOTE: This class is now obsolete. please use GridPivotTable Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
Uses the PivotCache method to return a PivotCache object for a PivotTable report (each report has only one cache). The source data of PivotCache come from WebWorksheet, DataTable, and so on.
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
