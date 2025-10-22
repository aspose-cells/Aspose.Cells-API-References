##Aspose::Cells::Cells class
'Aspose::Cells::Cells class. Encapsulates a collection of cell relevant objects, such as Cell, Row, ...etc in C++.'
## Cells class
Encapsulates a collection of cell relevant objects, such as [Cell](../cell/), [Row](../row/), ...etc.
```cpp
class Cells
```
## Methods
| Method | Description |
| --- | --- |
| [AddRange(const Range\& rangeObject)](./addrange/) | Adds a range object reference to cells. |
| [ApplyColumnStyle(int32_t column, const Style\& style, const StyleFlag\& flag)](./applycolumnstyle/) | Applies formats for a whole column. |
| [ApplyRowStyle(int32_t row, const Style\& style, const StyleFlag\& flag)](./applyrowstyle/) | Applies formats for a whole row. |
| [ApplyStyle(const Style\& style, const StyleFlag\& flag)](./applystyle/) | Applies formats for a whole worksheet. |
| [Cells(Cells_Impl* impl)](./cells/) | Constructs from an implementation object. |
| [Cells(const Cells\& src)](./cells/) | Copy constructor. |
| [CheckCell(int32_t row, int32_t column)](./checkcell/) | Gets the [Cell](../cell/) element or null at the specified cell row index and column index. |
| [CheckColumn(int32_t columnIndex)](./checkcolumn/) | Gets the [Column](../column/) element or null at the specified column index. |
| [CheckRow(int32_t row)](./checkrow/) | Gets the [Row](../row/) element or null at the specified cell row index. |
| [Clear()](./clear/) | Clears all data of the worksheet. |
| [ClearContents(const CellArea\& range)](./clearcontents/) | Clears contents of a range. |
| [ClearContents(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./clearcontents/) | Clears contents of a range. |
| [ClearFormats(const CellArea\& range)](./clearformats/) | Clears formatting of a range. |
| [ClearFormats(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./clearformats/) | Clears formatting of a range. |
| [ClearMergedCells()](./clearmergedcells/) | Clears all merged ranges. |
| [ClearRange(const CellArea\& range)](./clearrange/) | Clears contents and formatting of a range. |
| [ClearRange(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./clearrange/) | Clears contents and formatting of a range. |
| [ConvertStringToNumericValue()](./convertstringtonumericvalue/) | Converts all string data in the worksheet to numeric value if possible. |
| [CopyColumn(const Cells\& sourceCells, int32_t sourceColumnIndex, int32_t destinationColumnIndex)](./copycolumn/) | Copies data and formats of a whole column. |
| [CopyColumns(const Cells\& sourceCells0, int32_t sourceColumnIndex, int32_t destinationColumnIndex, int32_t columnNumber, const PasteOptions\& pasteOptions)](./copycolumns/) | Copies data and formats of a whole column. |
| [CopyColumns(const Cells\& sourceCells0, int32_t sourceColumnIndex, int32_t destinationColumnIndex, int32_t columnNumber)](./copycolumns/) | Copies data and formats of a whole column. |
| [CopyColumns(const Cells\& sourceCells, int32_t sourceColumnIndex, int32_t sourceTotalColumns, int32_t destinationColumnIndex, int32_t destinationTotalColumns)](./copycolumns/) | Copies data and formats of the whole columns. |
| [CopyRow(const Cells\& sourceCells, int32_t sourceRowIndex, int32_t destinationRowIndex)](./copyrow/) | Copies data and formats of a whole row. |
| [CopyRows(const Cells\& sourceCells, int32_t sourceRowIndex, int32_t destinationRowIndex, int32_t rowNumber)](./copyrows/) | Copies data and formats of some whole rows. |
| [CopyRows(const Cells\& sourceCells0, int32_t sourceRowIndex, int32_t destinationRowIndex, int32_t rowNumber, const CopyOptions\& copyOptions)](./copyrows/) | Copies data and formats of some whole rows. |
| [CopyRows(const Cells\& sourceCells0, int32_t sourceRowIndex, int32_t destinationRowIndex, int32_t rowNumber, const CopyOptions\& copyOptions, const PasteOptions\& pasteOptions)](./copyrows/) | Copies data and formats of some whole rows. |
| [CreateRange(const U16String\& upperLeftCell, const U16String\& lowerRightCell)](./createrange/) | Creates a [Range](../range/) object from a range of cells. |
| [CreateRange(const char16_t* upperLeftCell, const char16_t* lowerRightCell)](./createrange/) | Creates a [Range](../range/) object from a range of cells. |
| [CreateRange(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns)](./createrange/) | Creates a [Range](../range/) object from a range of cells. |
| [CreateRange(const U16String\& address)](./createrange/) | Creates a [Range](../range/) object from an address of the range. |
| [CreateRange(const char16_t* address)](./createrange/) | Creates a [Range](../range/) object from an address of the range. |
| [CreateRange(int32_t firstIndex, int32_t number, bool isVertical)](./createrange/) | Creates a [Range](../range/) object from rows of cells or columns of cells. |
| [DeleteBlankColumns()](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. |
| [DeleteBlankColumns(const DeleteOptions\& options)](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. |
| [DeleteBlankRows()](./deleteblankrows/) | Delete all blank rows which do not contain any data or other object. |
| [DeleteBlankRows(const DeleteOptions\& options)](./deleteblankrows/) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
| [DeleteColumn(int32_t columnIndex, bool updateReference)](./deletecolumn/) | Deletes a column. |
| [DeleteColumn(int32_t columnIndex)](./deletecolumn/) | Deletes a column. |
| [DeleteColumns(int32_t columnIndex, int32_t totalColumns, bool updateReference)](./deletecolumns/) | Deletes several columns. |
| [DeleteColumns(int32_t columnIndex, int32_t totalColumns, const DeleteOptions\& options)](./deletecolumns/) | Deletes several columns. |
| [DeleteRange(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn, ShiftType shiftType)](./deleterange/) | Deletes a range of cells and shift cells according to the shift option. |
| [DeleteRow(int32_t rowIndex)](./deleterow/) | Deletes a row. |
| [DeleteRow(int32_t rowIndex, bool updateReference)](./deleterow/) | Deletes a row. |
| [DeleteRows(int32_t rowIndex, int32_t totalRows)](./deleterows/) | Deletes multiple rows. |
| [DeleteRows(int32_t rowIndex, int32_t totalRows, bool updateReference)](./deleterows/) | Deletes multiple rows in the worksheet. |
| [DeleteRows(int32_t rowIndex, int32_t totalRows, const DeleteOptions\& options)](./deleterows/) | Deletes multiple rows in the worksheet. |
| [Dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [EndCellInColumn(int32_t columnIndex)](./endcellincolumn/) | Gets the last cell in this column. |
| [EndCellInColumn(int32_t startRow, int32_t endRow, int32_t startColumn, int32_t endColumn)](./endcellincolumn/) | Gets the last cell with maximum column index in this range. |
| [EndCellInRow(int32_t rowIndex)](./endcellinrow/) | Gets the last cell in this row. |
| [EndCellInRow(int32_t startRow, int32_t endRow, int32_t startColumn, int32_t endColumn)](./endcellinrow/) | Gets the last cell with maximum row index in this range. |
| [ExportArray(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns)](./exportarray/) | Exports data in the [Cells](./) collection to a two-dimension array object. |
| [Find(const Aspose::Cells::Object\& what, const Cell\& previousCell)](./find/) | Finds the cell containing with the input object. |
| [Find(const Aspose::Cells::Object\& what, const Cell\& previousCell, const FindOptions\& findOptions)](./find/) | Finds the cell containing with the input object. |
| [Get(int32_t row, int32_t column)](./get/) | Gets the [Cell](../cell/) element at the specified cell row index and column index. |
| [Get(const U16String\& cellName)](./get/) | Gets the [Cell](../cell/) element at the specified cell name. |
| [Get(const char16_t* cellName)](./get/) | Gets the [Cell](../cell/) element at the specified cell name. |
| [GetCell(int32_t row, int32_t column)](./getcell/) |  **(Deprecated)** Gets the [Cell](../cell/) element or null at the specified cell row index and column index. |
| [GetCellDisplayStyle(int32_t row, int32_t column)](./getcelldisplaystyle/) | Get the display style of given cell. |
| [GetCellDisplayStyle(int32_t row, int32_t column, BorderType adjacentBorders)](./getcelldisplaystyle/) | Get the display style of given cell. |
| [GetCellStyle(int32_t row, int32_t column)](./getcellstyle/) | Get the style of given cell. |
| [GetCellsWithPlaceInCellPicture()](./getcellswithplaceincellpicture/) | Gets all cells that contain embedded picture. |
| [GetColumnOriginalWidthPoint(int32_t column)](./getcolumnoriginalwidthpoint/) |  **(Deprecated)** Gets original column's height in unit of point if the column is hidden. |
| [GetColumns()](./getcolumns/) | Gets the collection of [Column](../column/) objects that represents the individual columns in this worksheet. |
| [GetColumnWidth(int32_t column, bool isOriginal, CellsUnitType unitType)](./getcolumnwidth/) | Gets the column width. |
| [GetColumnWidth(int32_t column)](./getcolumnwidth/) | Gets the width(in unit of characters) of the specified column in normal view. |
| [GetColumnWidthInch(int32_t column)](./getcolumnwidthinch/) |  **(Deprecated)** Gets the width of the specified column in normal view, in units of inches. |
| [GetColumnWidthPixel(int32_t column)](./getcolumnwidthpixel/) | Gets the width of the specified column in normal view, in units of pixel. |
| [GetColumnWidthPixel(int32_t column, bool original)](./getcolumnwidthpixel/) |  **(Deprecated)** Gets the width of the specified column in normal view, in units of pixel. |
| [GetCount()](./getcount/) | Gets the total count of instantiated [Cell](../cell/) objects. |
| [GetCountLarge()](./getcountlarge/) | Gets the total count of instantiated [Cell](../cell/) objects. |
| [GetDependents(bool isAll, int32_t row, int32_t column)](./getdependents/) | Get all cells which refer to the specific cell. |
| [GetDependentsInCalculation(int32_t row, int32_t column, bool recursive)](./getdependentsincalculation/) | Gets all cells whose calculated result depends on specific cell. |
| [GetEnumerator()](./getenumerator/) | Gets the cells enumerator. |
| [GetFirstCell()](./getfirstcell/) | Gets the first cell in this worksheet. |
| [GetFirstDataRow(int32_t column)](./getfirstdatarow/) | Gets the first row index of cell which contains data in the specified column. |
| [GetGroupedColumnOutlineLevel(int32_t columnIndex)](./getgroupedcolumnoutlinelevel/) | Gets the outline level (zero-based) of the column. |
| [GetGroupedRowOutlineLevel(int32_t rowIndex)](./getgroupedrowoutlinelevel/) | Gets the outline level (zero-based) of the row. |
| [GetLastCell()](./getlastcell/) | Gets the last cell in this worksheet. |
| [GetLastDataRow(int32_t column)](./getlastdatarow/) | Gets the last row index of cell which contains data in the specified column. |
| [GetMaxColumn()](./getmaxcolumn/) | Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [GetMaxDataColumn()](./getmaxdatacolumn/) | Maximum column index of cell which contains data. |
| [GetMaxDataRow()](./getmaxdatarow/) | Maximum row index of cell which contains data. |
| [GetMaxDisplayRange()](./getmaxdisplayrange/) | Gets the max range which includes data, merged cells and shapes. |
| [GetMaxGroupedColumnOutlineLevel()](./getmaxgroupedcolumnoutlinelevel/) | Gets the max grouped column outline level (zero-based). |
| [GetMaxGroupedRowOutlineLevel()](./getmaxgroupedrowoutlinelevel/) | Gets the max grouped row outline level (zero-based). |
| [GetMaxRow()](./getmaxrow/) | Maximum row index of cell which contains data or style. |
| [GetMemorySetting()](./getmemorysetting/) | Gets or sets the memory usage option for this cells. |
| [GetMergedAreas()](./getmergedareas/) | Gets all merged cells. |
| [GetMinColumn()](./getmincolumn/) | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [GetMinDataColumn()](./getmindatacolumn/) | Minimum column index of cell which contains data. |
| [GetMinDataRow()](./getmindatarow/) | Minimum row index of cell which contains data. |
| [GetMinRow()](./getminrow/) | Minimum row index of cell which contains data or style. |
| [GetMultiThreadReading()](./getmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [GetOdsCellFields()](./getodscellfields/) | Gets the list of fields of ods. |
| [GetPreserveString()](./getpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [GetRanges()](./getranges/) | Gets the collection of [Range](../range/) objects created at run time. |
| [GetRow(int32_t row)](./getrow/) |  **(Deprecated)** Gets the [Row](../row/) element at the specified cell row index. |
| [GetRowHeight(int32_t row, bool isOriginal, CellsUnitType unitType)](./getrowheight/) | Gets row's height. |
| [GetRowHeight(int32_t row)](./getrowheight/) | Gets the height of a specified row, in unit of points. |
| [GetRowHeightInch(int32_t row)](./getrowheightinch/) | Gets the height of a specified row in unit of inches. |
| [GetRowHeightPixel(int32_t row)](./getrowheightpixel/) | Gets the height of a specified row in unit of pixel. |
| [GetRowOriginalHeightPoint(int32_t row)](./getroworiginalheightpoint/) |  **(Deprecated)** Gets original row's height in unit of point if the row is hidden. |
| [GetRows()](./getrows/) | Gets the collection of [Row](../row/) objects that represents the individual rows in this worksheet. |
| [GetStandardHeight()](./getstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
| [GetStandardHeightInch()](./getstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [GetStandardHeightPixels()](./getstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [GetStandardWidth()](./getstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [GetStandardWidthInch()](./getstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [GetStandardWidthPixels()](./getstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [GetStyle()](./getstyle/) | Gets and sets the default style of the worksheet. |
| [GetViewColumnWidthPixel(int32_t column)](./getviewcolumnwidthpixel/) | Get the width in different view type. |
| [GetViewRowHeight(int32_t row)](./getviewrowheight/) | Gets the height of a specified row. |
| [GetViewRowHeightInch(int32_t row)](./getviewrowheightinch/) | Gets the height of a specified row in unit of inches. |
| [GroupColumns(int32_t firstIndex, int32_t lastIndex)](./groupcolumns/) | Groups columns. |
| [GroupColumns(int32_t firstIndex, int32_t lastIndex, bool isHidden)](./groupcolumns/) | Groups columns. |
| [GroupRows(int32_t firstIndex, int32_t lastIndex, bool isHidden)](./grouprows/) | Groups rows. |
| [GroupRows(int32_t firstIndex, int32_t lastIndex)](./grouprows/) | Groups rows. |
| [HideColumn(int32_t column)](./hidecolumn/) | Hides a column. |
| [HideColumns(int32_t column, int32_t totalColumns)](./hidecolumns/) | Hide multiple columns. |
| [HideGroupDetail(bool isVertical, int32_t index)](./hidegroupdetail/) | Collapses the grouped rows/columns. |
| [HideRow(int32_t row)](./hiderow/) | Hides a row. |
| [HideRows(int32_t row, int32_t totalRows)](./hiderows/) | Hides multiple rows. |
| [ImportCSV(const U16String\& fileName, const U16String\& splitter, bool convertNumericData, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const char16_t* fileName, const char16_t* splitter, bool convertNumericData, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const Vector \<uint8_t\>\& stream, const U16String\& splitter, bool convertNumericData, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const Vector \<uint8_t\>\& stream, const char16_t* splitter, bool convertNumericData, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const U16String\& fileName, const TxtLoadOptions\& options, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const char16_t* fileName, const TxtLoadOptions\& options, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportCSV(const Vector \<uint8_t\>\& stream, const TxtLoadOptions\& options, int32_t firstRow, int32_t firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [ImportFormulaArray(const Vector \<U16String\>\& stringArray, int32_t firstRow, int32_t firstColumn, bool isVertical)](./importformulaarray/) | Imports an array of formula into a worksheet. |
| [InsertColumn(int32_t columnIndex, bool updateReference)](./insertcolumn/) | Inserts a new column into the worksheet. |
| [InsertColumn(int32_t columnIndex)](./insertcolumn/) | Inserts a new column into the worksheet. |
| [InsertColumns(int32_t columnIndex, int32_t totalColumns)](./insertcolumns/) | Inserts some columns into the worksheet. |
| [InsertColumns(int32_t columnIndex, int32_t totalColumns, bool updateReference)](./insertcolumns/) | Inserts some columns into the worksheet. |
| [InsertColumns(int32_t columnIndex, int32_t totalColumns, const InsertOptions\& options)](./insertcolumns/) | Inserts some columns into the worksheet. |
| [InsertCutCells(const Range\& cutRange, int32_t row, int32_t column, ShiftType shiftType)](./insertcutcells/) | Insert cut range. |
| [InsertRange(const CellArea\& area, int32_t shiftNumber, ShiftType shiftType, bool updateReference)](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange(const CellArea\& area, ShiftType shiftType)](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange(const CellArea\& area, int32_t shiftNumber, ShiftType shiftType)](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRow(int32_t rowIndex)](./insertrow/) | Inserts a new row into the worksheet. |
| [InsertRows(int32_t rowIndex, int32_t totalRows, bool updateReference)](./insertrows/) | Inserts multiple rows into the worksheet. |
| [InsertRows(int32_t rowIndex, int32_t totalRows, const InsertOptions\& options)](./insertrows/) | Inserts multiple rows into the worksheet. |
| [InsertRows(int32_t rowIndex, int32_t totalRows)](./insertrows/) | Inserts multiple rows into the worksheet. |
| [IsBlankColumn(int32_t columnIndex)](./isblankcolumn/) | Checks whether given column is blank(does not contain any data). |
| [IsColumnHidden(int32_t columnIndex)](./iscolumnhidden/) | Checks whether a column at given index is hidden. |
| [IsDefaultColumnHidden()](./isdefaultcolumnhidden/) |  |
| [IsDefaultRowHeightMatched()](./isdefaultrowheightmatched/) | Indicates that row height and default font height matches. |
| [IsDefaultRowHidden()](./isdefaultrowhidden/) | Indicates whether the row is default hidden. |
| [IsDeletingRangeEnabled(int32_t startRow, int32_t startColumn, int32_t totalRows, int32_t totalColumns)](./isdeletingrangeenabled/) | Check whether the range could be deleted. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRowHidden(int32_t rowIndex)](./isrowhidden/) | Checks whether a row at given index is hidden. |
| [LinkToXmlMap(const U16String\& mapName, int32_t row, int32_t column, const U16String\& path)](./linktoxmlmap/) | Link to a xml map. |
| [LinkToXmlMap(const char16_t* mapName, int32_t row, int32_t column, const char16_t* path)](./linktoxmlmap/) | Link to a xml map. |
| [Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns)](./merge/) | Merges a specified range of cells into a single cell. |
| [Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, bool mergeConflict)](./merge/) | Merges a specified range of cells into a single cell. |
| [Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, bool checkConflict, bool mergeConflict)](./merge/) | Merges a specified range of cells into a single cell. |
| [MoveRange(const CellArea\& sourceArea, int32_t destRow, int32_t destColumn)](./moverange/) | Moves the range. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Cells\& src)](./operator_asm/) | operator= |
| [RemoveDuplicates()](./removeduplicates/) | Removes duplicate rows in the sheet. |
| [RemoveDuplicates(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./removeduplicates/) | Removes duplicate values in the range. |
| [RemoveDuplicates(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn, bool hasHeaders, const Vector \<int32_t\>\& columnOffsets)](./removeduplicates/) | Removes duplicate data of the range. |
| [RemoveFormulas()](./removeformulas/) | Removes all formula and replaces with the value of the formula. |
| [RetrieveSubtotalSetting(const CellArea\& ca)](./retrievesubtotalsetting/) | Retrieves subtotals setting of the range. |
| [SetColumnWidth(int32_t column, double width)](./setcolumnwidth/) | Sets the width of the specified column in normal view. |
| [SetColumnWidthInch(int32_t column, double inches)](./setcolumnwidthinch/) | Sets column width in unit of inches in normal view. |
| [SetColumnWidthPixel(int32_t column, int32_t pixels)](./setcolumnwidthpixel/) | Sets column width in unit of pixels in normal view. |
| [SetIsDefaultColumnHidden(bool value)](./setisdefaultcolumnhidden/) |  |
| [SetIsDefaultRowHeightMatched(bool value)](./setisdefaultrowheightmatched/) | Indicates that row height and default font height matches. |
| [SetIsDefaultRowHidden(bool value)](./setisdefaultrowhidden/) | Indicates whether the row is default hidden. |
| [SetMemorySetting(MemorySetting value)](./setmemorysetting/) | Gets or sets the memory usage option for this cells. |
| [SetMultiThreadReading(bool value)](./setmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [SetPreserveString(bool value)](./setpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [SetRowHeight(int32_t row, double height)](./setrowheight/) | Sets the height of the specified row. |
| [SetRowHeightInch(int32_t row, double inches)](./setrowheightinch/) | Sets row height in unit of inches. |
| [SetRowHeightPixel(int32_t row, int32_t pixels)](./setrowheightpixel/) | Sets row height in unit of pixels. |
| [SetStandardHeight(double value)](./setstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
| [SetStandardHeightInch(double value)](./setstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [SetStandardHeightPixels(int32_t value)](./setstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [SetStandardWidth(double value)](./setstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [SetStandardWidthInch(double value)](./setstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [SetStandardWidthPixels(int32_t value)](./setstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [SetStyle(const Style\& value)](./setstyle/) | Gets and sets the default style of the worksheet. |
| [SetViewColumnWidthPixel(int32_t column, int32_t pixels)](./setviewcolumnwidthpixel/) | Sets the width of the column in different view. |
| [ShowGroupDetail(bool isVertical, int32_t index)](./showgroupdetail/) | Expands the grouped rows/columns. |
| [Subtotal(const CellArea\& ca, int32_t groupBy, ConsolidationFunction function, const Vector \<int32_t\>\& totalList)](./subtotal/) | Creates subtotals for the range. |
| [Subtotal(const CellArea\& ca, int32_t groupBy, ConsolidationFunction function, const Vector \<int32_t\>\& totalList, bool replace, bool pageBreaks, bool summaryBelowData)](./subtotal/) | Creates subtotals for the range. |
| [TextToColumns(int32_t row, int32_t column, int32_t totalRows, const TxtLoadOptions\& options)](./texttocolumns/) | Splits content in specified column into multiple columns.. |
| [UngroupColumns(int32_t firstIndex, int32_t lastIndex)](./ungroupcolumns/) | Ungroups columns. |
| [UngroupRows(int32_t firstIndex, int32_t lastIndex, bool isAll)](./ungrouprows/) | Ungroups rows. |
| [UngroupRows(int32_t firstIndex, int32_t lastIndex)](./ungrouprows/) | Ungroups rows. |
| [UnhideColumn(int32_t column, double width)](./unhidecolumn/) | Unhides a column. |
| [UnhideColumns(int32_t column, int32_t totalColumns, double width)](./unhidecolumns/) | Unhide multiple columns. |
| [UnhideRow(int32_t row, double height)](./unhiderow/) | Unhides a row. |
| [UnhideRows(int32_t row, int32_t totalRows, double height)](./unhiderows/) | Unhides the hidden rows. |
| [UnMerge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns)](./unmerge/) | Unmerges a specified range of merged cells. |
| [~Cells()](./~cells/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
//Set default row height
cells.SetStandardHeight(20);
//Set row height
cells.SetRowHeight(2, 20.5);
//Set default colum width
cells.SetStandardWidth(15);
//Set column width
cells.SetColumnWidth(3, 12.57);
//Merge cells
cells.Merge(5, 4, 2, 2);
//Put values to cells
cells.Get(0, 0).PutValue(true);
cells.Get(0, 1).PutValue(1);
cells.Get(0, 2).PutValue(u"abc");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
