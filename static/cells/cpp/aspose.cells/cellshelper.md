##Aspose::Cells::CellsHelper class
'Aspose::Cells::CellsHelper class. Provides helper functions in C++.'
## CellsHelper class
Provides helper functions.
```cpp
class CellsHelper
```
## Methods
| Method | Description |
| --- | --- |
| static [CellIndexToName(int32_t row, int32_t column)](./cellindextoname/) | Gets cell name according to its row and column indexes. |
| static [CellNameToIndex(const U16String\& cellName, int32_t\& row, int32_t\& column)](./cellnametoindex/) | Gets the cell row and column indexes according to its name. |
| static [CellNameToIndex(const char16_t* cellName, int32_t\& row, int32_t\& column)](./cellnametoindex/) | Gets the cell row and column indexes according to its name. |
| static [ColumnIndexToName(int32_t column)](./columnindextoname/) | Gets column name according to column index. |
| static [ColumnNameToIndex(const U16String\& columnName)](./columnnametoindex/) | Gets column index according to column name. |
| static [ColumnNameToIndex(const char16_t* columnName)](./columnnametoindex/) | Gets column index according to column name. |
| static [CreateSafeSheetName(const U16String\& nameProposal)](./createsafesheetname/) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value. |
| static [CreateSafeSheetName(const char16_t* nameProposal)](./createsafesheetname/) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value. |
| static [CreateSafeSheetName(const U16String\& nameProposal, char16_t replaceChar)](./createsafesheetname/) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value. |
| static [CreateSafeSheetName(const char16_t* nameProposal, char16_t replaceChar)](./createsafesheetname/) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value. |
| static [GetAltStartPath()](./getaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| static [GetCacheFolder()](./getcachefolder/) | Gets the folder for temporary files that may be used as data cache. |
| static [GetDateTimeFromDouble(double doubleValue, bool date1904)](./getdatetimefromdouble/) | Convert the double value to the date time value. |
| static [GetDoubleFromDateTime(const Date\& dateTime, bool date1904)](./getdoublefromdatetime/) | Convert the date time to double value. |
| static [GetDPI()](./getdpi/) | Gets the DPI of the machine. |
| static [GetLibraryPath()](./getlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
| static [GetSignificantDigitsType()](./getsignificantdigitstype/) | Gets and sets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G17](../significantdigitstype/). |
| static [GetStartupPath()](./getstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
| static [GetTextWidth(const U16String\& text, const Aspose::Cells::Font\& font, double scaling)](./gettextwidth/) | Get width of text in unit of points. |
| static [GetTextWidth(const char16_t* text, const Aspose::Cells::Font\& font, double scaling)](./gettextwidth/) | Get width of text in unit of points. |
| static [GetUsedColors(const Workbook\& workbook)](./getusedcolors/) | Gets all used colors in the workbook. |
| static [GetVersion()](./getversion/) | Get the release version. |
| static [IsCloudPlatform()](./iscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,. |
| static [MergeFiles(const Vector \<U16String\>\& files, const U16String\& cachedFile, const U16String\& destFile)](./mergefiles/) | Merges some large xls files to a xls file. |
| static [MergeFiles(const Vector \<U16String\>\& files, const char16_t* cachedFile, const char16_t* destFile)](./mergefiles/) | Merges some large xls files to a xls file. |
| static [NeedQuoteInFormula(const U16String\& sheetName)](./needquoteinformula/) | Indicates whether the name of the sheet should be enclosed in single quotes. |
| static [NeedQuoteInFormula(const char16_t* sheetName)](./needquoteinformula/) | Indicates whether the name of the sheet should be enclosed in single quotes. |
| static [RowIndexToName(int32_t row)](./rowindextoname/) | Gets row name according to row index. |
| static [RowNameToIndex(const U16String\& rowName)](./rownametoindex/) | Gets row index according to row name. |
| static [RowNameToIndex(const char16_t* rowName)](./rownametoindex/) | Gets row index according to row name. |
| static [SetAltStartPath(const U16String\& value)](./setaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| static [SetAltStartPath(const char16_t* value)](./setaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| static [SetCacheFolder(const U16String\& cache)](./setcachefolder/) | Sets the folder for temporary files that may be used as data cache. |
| static [SetCacheFolder(const char16_t* cache)](./setcachefolder/) | Sets the folder for temporary files that may be used as data cache. |
| static [SetDPI(double value)](./setdpi/) | Gets the DPI of the machine. |
| static [SetIsCloudPlatform(bool value)](./setiscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,. |
| static [SetLibraryPath(const U16String\& value)](./setlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
| static [SetLibraryPath(const char16_t* value)](./setlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
| static [SetSignificantDigitsType(SignificantDigitsType value)](./setsignificantdigitstype/) | Gets and sets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G17](../significantdigitstype/). |
| static [SetStartupPath(const U16String\& value)](./setstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
| static [SetStartupPath(const char16_t* value)](./setstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
