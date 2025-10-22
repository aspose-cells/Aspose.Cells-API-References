##Aspose::Cells::ImportTableOptions class
'Aspose::Cells::ImportTableOptions class. Represents the options of importing data into cells in C++.'
## ImportTableOptions class
Represents the options of importing data into cells.
```cpp
class ImportTableOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetCheckMergedCells()](./getcheckmergedcells/) | Indicates whether checking merged cells. |
| [GetColumnIndexes()](./getcolumnindexes/) | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [GetConvertGridStyle()](./getconvertgridstyle/) | Indicates whether apply the style of the grid view to cells. |
| [GetConvertNumericData()](./getconvertnumericdata/) | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [GetDateFormat()](./getdateformat/) | Gets or sets date format string for cells with imported datetime values. |
| [GetDefaultValues()](./getdefaultvalues/) | Default value for the value in the table is null. |
| [GetExportCaptionAsFieldName()](./getexportcaptionasfieldname/) | Indicates whether exporting caption as field name. |
| [GetInsertRows()](./getinsertrows/) | Indicates whether new rows should be added for importing data records. |
| [GetIsFormulas()](./getisformulas/) | Indicates whether the data are formulas. |
| [GetNumberFormats()](./getnumberformats/) | Gets or sets the number formats. |
| [GetShiftFirstRowDown()](./getshiftfirstrowdown/) | Indicates whether shifting the first row down when inserting rows. |
| [GetTotalColumns()](./gettotalcolumns/) | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [GetTotalRows()](./gettotalrows/) | Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [ImportTableOptions()](./importtableoptions/) | Creates the default importing options. |
| [ImportTableOptions(ImportTableOptions_Impl* impl)](./importtableoptions/) | Constructs from an implementation object. |
| [ImportTableOptions(const ImportTableOptions\& src)](./importtableoptions/) | Copy constructor. |
| [IsFieldNameShown()](./isfieldnameshown/) | Indicates whether field name should be imported. |
| [IsHtmlString()](./ishtmlstring/) | Indicates whether the value contains html tags. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ImportTableOptions\& src)](./operator_asm/) | operator= |
| [SetCheckMergedCells(bool value)](./setcheckmergedcells/) | Indicates whether checking merged cells. |
| [SetColumnIndexes(const Vector \<int32_t\>\& value)](./setcolumnindexes/) | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [SetConvertGridStyle(bool value)](./setconvertgridstyle/) | Indicates whether apply the style of the grid view to cells. |
| [SetConvertNumericData(bool value)](./setconvertnumericdata/) | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [SetDateFormat(const U16String\& value)](./setdateformat/) | Gets or sets date format string for cells with imported datetime values. |
| [SetDateFormat(const char16_t* value)](./setdateformat/) | Gets or sets date format string for cells with imported datetime values. |
| [SetDefaultValues(const Vector \<Aspose::Cells::Object\>\& value)](./setdefaultvalues/) | Default value for the value in the table is null. |
| [SetExportCaptionAsFieldName(bool value)](./setexportcaptionasfieldname/) | Indicates whether exporting caption as field name. |
| [SetInsertRows(bool value)](./setinsertrows/) | Indicates whether new rows should be added for importing data records. |
| [SetIsFieldNameShown(bool value)](./setisfieldnameshown/) | Indicates whether field name should be imported. |
| [SetIsFormulas(const Vector \<bool\>\& value)](./setisformulas/) | Indicates whether the data are formulas. |
| [SetIsHtmlString(bool value)](./setishtmlstring/) | Indicates whether the value contains html tags. |
| [SetNumberFormats(const Vector \<U16String\>\& value)](./setnumberformats/) | Gets or sets the number formats. |
| [SetShiftFirstRowDown(bool value)](./setshiftfirstrowdown/) | Indicates whether shifting the first row down when inserting rows. |
| [SetTotalColumns(int32_t value)](./settotalcolumns/) | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [SetTotalRows(int32_t value)](./settotalrows/) | Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [~ImportTableOptions()](./~importtableoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
