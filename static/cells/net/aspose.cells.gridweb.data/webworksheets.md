##Class WebWorksheets
Aspose.Cells.GridWeb.Data.WebWorksheets class.
## WebWorksheets class
```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |
## Properties
| Name | Description |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Gets a value indicating whether the collection has a fixed size. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Gets a value indicating whether the IList is read-only. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Gets a value indicating if access to the ICollection is synchronized (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Gets the Worksheet element at the specified index. (2 indexers) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Gets the PivotCache collection object |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Gets the pivotTable collection object. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Gets an object that can be used to synchronize access to the ICollection. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Adds a worksheet to the collection. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Adds a sheet object. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Adds a worksheet to the collection. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Adds a worksheet to the collection and copys data from an existed worksheet. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Adds a worksheet to the collection and copys data from an existed worksheet. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Clear all worksheets. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Indicates whether the collection contains the sheet. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Copys contents to an array. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Imports from a DataView. Creates a sheet with the DataView's table name automatically. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Imports from a DataView to the specified sheet and position. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Imports from an excel file stream, including disk file stream or memory stream. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Imports from an excel file. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Gets the index of the sheet. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Inserts a sheet to the index. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Loads data from a CSV file stream. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Loads data from a CSV file. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Loads data from a HTML file stream. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Loads data from a HTML file. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Loads data from a SpreadSheetML file stream. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Loads data from a SpreadSheetML file. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Removes a sheet. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Removes a sheet at the index. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Removes the element at a specified name. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Runs all the cells's formula. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Saves data to a CSV file stream. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Saves data to a CSV file. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Saves data to a HTML file stream. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Saves data to a HTML file. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Saves data to a SpreadSheetML file stream. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Saves data to a SpreadSheetML file. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Saves the worksheets to a excel file stream, including disk IO stream or memory stream. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Saves the worksheets to an excel file with Excel 2003 format. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Saves the worksheets to an excel file. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Saves the worksheets to an excel file. |
### Remarks
NOTE: This class is now obsolete. please use GridWorksheetCollection Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
