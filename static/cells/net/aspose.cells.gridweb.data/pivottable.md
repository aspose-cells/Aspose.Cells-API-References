##Class PivotTable
Aspose.Cells.GridWeb.Data.PivotTable class. Represents a PivotTable report on a worksheet. The PivotTable object is a member of the PivotTables collection. The PivotTables collection contains all the PivotTable objects on a control
## PivotTable class
Represents a PivotTable report on a worksheet. The PivotTable object is a member of the [`PivotTables`](../pivottables/) collection. The PivotTables collection contains all the PivotTable objects on a control.
```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotTable
```
## Properties
| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.gridweb.data/pivottable/name/) { get; } | Gets name |
| [PivotCache](../../aspose.cells.gridweb.data/pivottable/pivotcache/) { get; } | Gets PivotCache object that the report used. |
| [PivotFields](../../aspose.cells.gridweb.data/pivottable/pivotfields/) { get; } | Repesents all fields in PivotTable report. |
## Methods
| Name | Description |
| --- | --- |
| [DataBind](../../aspose.cells.gridweb.data/pivottable/databind/)() |  |
### Remarks
NOTE: This class is now obsolete. please use GridPivotTable Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
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
