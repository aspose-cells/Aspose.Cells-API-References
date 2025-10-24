##Class RowFilterSettings
Aspose.Cells.GridWeb.Data.RowFilterSettings class. Summary description for RowFilter
## RowFilterSettings class
Summary description for RowFilter.
```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```
## Properties
| Name | Description |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | The filter criteria string. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Enables auto filtering. The HeaderRow will display dropdown buttons to let user select the column's value to be filtered. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | The end row number of the filter range. If this value is set to -1, the last row number of the sheet is used. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | The header row number which will display filter dropdown buttons. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | The start row number of the filter range. |
## Methods
| Name | Description |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Builds criteria string from auto filter settings. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Clears all filter settings and display all rows. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Specifies a custom filter. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filters rows using criteria string. |
### Remarks
NOTE: This class is now obsolete. This class will be removed after 6 months since Aug. 2014. you can use GridWorksheet AddAutoFilter/FilterString for autofilter /custom filter settings Aspose apologizes for any inconvenience you may have experienced.
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
