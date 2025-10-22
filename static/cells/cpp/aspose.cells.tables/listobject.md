##Aspose::Cells::Tables::ListObject class
'Aspose::Cells::Tables::ListObject class. Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet in C++.'
## ListObject class
Represents a list object on a worksheet. The [ListObject](./) object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.
```cpp
class ListObject
```
## Methods
| Method | Description |
| --- | --- |
| [ApplyStyleToRange()](./applystyletorange/) | Apply the table style to the range. |
| [ConvertToRange()](./converttorange/) | Convert the table to range. |
| [ConvertToRange(const TableToRangeOptions\& options)](./converttorange/) | Convert the table to range. |
| [Filter()](./filter/) | Filter the table. |
| [GetAlternativeDescription()](./getalternativedescription/) | Gets and sets the alternative description. |
| [GetAlternativeText()](./getalternativetext/) | Gets and sets the alternative text. |
| [GetAutoFilter()](./getautofilter/) | Gets auto filter. |
| [GetComment()](./getcomment/) | Gets and sets the comment of the table. |
| [GetDataRange()](./getdatarange/) | Gets the data range of the [ListObject](./). |
| [GetDataSourceType()](./getdatasourcetype/) | Gets the data source type of the table. |
| [GetDisplayName()](./getdisplayname/) | Gets and sets the display name. |
| [GetEndColumn()](./getendcolumn/) | Gets the end column of the range. |
| [GetEndRow()](./getendrow/) | Gets the end row of the range. |
| [GetListColumns()](./getlistcolumns/) | Gets ListColumns of the [ListObject](./). |
| [GetQueryTable()](./getquerytable/) | Gets the linked [QueryTable](../../aspose.cells/querytable/). |
| [GetShowHeaderRow()](./getshowheaderrow/) | Gets and sets whether this [ListObject](./) show header row. |
| [GetShowTableStyleColumnStripes()](./getshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
| [GetShowTableStyleFirstColumn()](./getshowtablestylefirstcolumn/) | Indicates whether the first column in the table should have the style applied. |
| [GetShowTableStyleLastColumn()](./getshowtablestylelastcolumn/) | Indicates whether the last column in the table should have the style applied. |
| [GetShowTableStyleRowStripes()](./getshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied. |
| [GetShowTotals()](./getshowtotals/) | Gets and sets whether this [ListObject](./) show total row. |
| [GetStartColumn()](./getstartcolumn/) | Gets the start column of the range. |
| [GetStartRow()](./getstartrow/) | Gets the start row of the range. |
| [GetTableStyleName()](./gettablestylename/) | Gets and sets the table style name. |
| [GetTableStyleType()](./gettablestyletype/) | Gets and the built-in table style. |
| [GetXmlMap()](./getxmlmap/) | Gets an [XmlMap](../../aspose.cells/xmlmap/) used for this list. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [ListObject(ListObject_Impl* impl)](./listobject/) | Constructs from an implementation object. |
| [ListObject(const ListObject\& src)](./listobject/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ListObject\& src)](./operator_asm/) | operator= |
| [PutCellFormula(int32_t rowOffset, int32_t columnOffset, const U16String\& formula)](./putcellformula/) | Put the formula to the cell in the table. |
| [PutCellFormula(int32_t rowOffset, int32_t columnOffset, const char16_t* formula)](./putcellformula/) | Put the formula to the cell in the table. |
| [PutCellFormula(int32_t rowOffset, int32_t columnOffset, const U16String\& formula, bool isTotalsRowFormula)](./putcellformula/) | Put the formula to the cell in the table. |
| [PutCellFormula(int32_t rowOffset, int32_t columnOffset, const char16_t* formula, bool isTotalsRowFormula)](./putcellformula/) | Put the formula to the cell in the table. |
| [PutCellValue(int32_t rowOffset, int32_t columnOffset, const Aspose::Cells::Object\& value)](./putcellvalue/) | Put the value to the cell. |
| [PutCellValue(int32_t rowOffset, int32_t columnOffset, const Aspose::Cells::Object\& value, bool isTotalsRowLabel)](./putcellvalue/) | Put the value to the cell. |
| [Resize(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn, bool hasHeaders)](./resize/) | Resize the range of the list object. |
| [SetAlternativeDescription(const U16String\& value)](./setalternativedescription/) | Gets and sets the alternative description. |
| [SetAlternativeDescription(const char16_t* value)](./setalternativedescription/) | Gets and sets the alternative description. |
| [SetAlternativeText(const U16String\& value)](./setalternativetext/) | Gets and sets the alternative text. |
| [SetAlternativeText(const char16_t* value)](./setalternativetext/) | Gets and sets the alternative text. |
| [SetComment(const U16String\& value)](./setcomment/) | Gets and sets the comment of the table. |
| [SetComment(const char16_t* value)](./setcomment/) | Gets and sets the comment of the table. |
| [SetDisplayName(const U16String\& value)](./setdisplayname/) | Gets and sets the display name. |
| [SetDisplayName(const char16_t* value)](./setdisplayname/) | Gets and sets the display name. |
| [SetShowHeaderRow(bool value)](./setshowheaderrow/) | Gets and sets whether this [ListObject](./) show header row. |
| [SetShowTableStyleColumnStripes(bool value)](./setshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
| [SetShowTableStyleFirstColumn(bool value)](./setshowtablestylefirstcolumn/) | Indicates whether the first column in the table should have the style applied. |
| [SetShowTableStyleLastColumn(bool value)](./setshowtablestylelastcolumn/) | Indicates whether the last column in the table should have the style applied. |
| [SetShowTableStyleRowStripes(bool value)](./setshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied. |
| [SetShowTotals(bool value)](./setshowtotals/) | Gets and sets whether this [ListObject](./) show total row. |
| [SetTableStyleName(const U16String\& value)](./settablestylename/) | Gets and sets the table style name. |
| [SetTableStyleName(const char16_t* value)](./settablestylename/) | Gets and sets the table style name. |
| [SetTableStyleType(TableStyleType value)](./settablestyletype/) | Gets and the built-in table style. |
| [UpdateColumnName()](./updatecolumnname/) | Updates all list columns' name from the worksheet. |
| [~ListObject()](./~listobject/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
for (int i = 0; i < 5; i++)
{
cells.Get(0, i).PutValue(CellsHelper::ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 5; column++)
{
cells.Get(row, column).PutValue(row * column);
}
}
ListObjectCollection tables = workbook.GetWorksheets().Get(0).GetListObjects();
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables.Get(0);
table.SetShowTotals(true);
table.GetListColumns().Get(4).SetTotalsCalculation(TotalsCalculation::Sum);
workbook.Save(u"Book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Tables](../)
* Library [Aspose.Cells for C++](../../)
