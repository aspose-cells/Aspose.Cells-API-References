##CellsHelper Class
'CellsHelper class. Encapsulates the object that represents cellshelper in Go.'
## CellsHelper class
Provides helper functions.
```go
type CellsHelper struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Gets and sets the default type of significant digits for outputing numeric values.Default value is SignificantDigitsType.G17. |
|[CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Gets and sets the default type of significant digits for outputing numeric values.Default value is SignificantDigitsType.G17. |
|[CellsHelper_GetDPI](./cellshelper_getdpi/) | Gets the DPI of the machine. |
|[CellsHelper_SetDPI](./cellshelper_setdpi/) | Gets the DPI of the machine. |
|[CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Get width of text in unit of points. |
|[CellsHelper_GetVersion](./cellshelper_getversion/) | Get the release version. |
|[CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Gets the cell row and column indexes according to its name. |
|[CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Gets cell name according to its row and column indexes. |
|[CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Gets column name according to column index. |
|[CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Gets column index according to column name. |
|[CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Gets row name according to row index. |
|[CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Gets row index according to row name. |
|[CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Convert the double value to the date time value. |
|[CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Convert the date time to double value. |
|[CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
|[CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
|[CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
|[CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
|[CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
|[CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
|[CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Gets all used colors in the workbook. |
|[CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Merges some large xls files to a xls file. |
|[CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Gets the folder for temporary files that may be used as data cache. |
|[CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Sets the folder for temporary files that may be used as data cache. |
|[CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with ' ', then return the rebuilt string value. |
|[CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with given character, then return the rebuilt string value. |
|[CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Indicates whether the name of the sheet should be enclosed in single quotes |
|[CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
|[CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
