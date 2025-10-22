##PivotCache.SourceCellArea
PivotCache property. Returns the range of the data source using with SourceSheet
## PivotCache.SourceCellArea property
Returns the range of the data source using with SourceSheet.
```csharp
public WebCellArea SourceCellArea { get; }
```
### Examples
```csharp
[C#]
//Changes data source range
//Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
//Adds 2 row data
table.PivotCache.SourceCellArea.EndRow = 12;
[VB]
'Changes data source range
'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
'Adds 2 row data
table.PivotCache.SourceCellArea.EndRow = 12
```
### See Also
* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
