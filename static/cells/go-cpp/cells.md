##Cells Class
'Cells class. Encapsulates the object that represents cells in Go.'
## Cells class
Encapsulates a collection of cell relevant objects, such as <see cref="Cell"/>, <see cref="Row"/>, ...etc.
```go
type Cells struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOdsCellFields](./getodscellfields/) | Gets the list of fields of ods. |
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. |
|[GetCount](./getcount/) | Gets the total count of instantiated Cell objects. |
|[GetCountLarge](./getcountlarge/) | Gets the total count of instantiated Cell objects. |
|[GetEnumerator](./getenumerator/) | Gets the cells enumerator. |
|[GetRows](./getrows/) | Gets the collection of Row objects that represents the individual rows in this worksheet. |
|[GetMergedAreas](./getmergedareas/) | Gets all merged cells. |
|[CheckCell](./checkcell/) | Gets the Cell element or null at the specified cell row index and column index. |
|[CheckRow](./checkrow/) | Gets the Row element or null at the specified cell row index. |
|[CheckColumn](./checkcolumn/) | Gets the Column element or null at the specified column index. |
|[IsRowHidden](./isrowhidden/) | Checks whether a row at given index is hidden. |
|[IsColumnHidden](./iscolumnhidden/) | Checks whether a column at given index is hidden. |
|[AddRange](./addrange/) | Adds a range object reference to cells |
|[CreateRange_String_String](./createrange_string_string/) | Creates a Range object from a range of cells. |
|[CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Creates a Range object from a range of cells. |
|[CreateRange_String](./createrange_string/) | Creates a Range object from an address of the range. |
|[CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Creates a Range object from rows of cells or columns of cells. |
|[Get_Int_Int](./get_int_int/) | Gets the Cell element at the specified cell row index and column index. |
|[Get_String](./get_string/) | Gets the Cell element at the specified cell name. |
|[GetMultiThreadReading](./getmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading.Default value of this property is false. |
|[SetMultiThreadReading](./setmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading.Default value of this property is false. |
|[GetMemorySetting](./getmemorysetting/) | Gets or sets the memory usage option for this cells. |
|[SetMemorySetting](./setmemorysetting/) | Gets or sets the memory usage option for this cells. |
|[Clear](./clear/) | Clears all data of the worksheet. |
|[GetStyle](./getstyle/) | Gets and sets the default style of the worksheet. |
|[SetStyle](./setstyle/) | Gets and sets the default style of the worksheet. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  |
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  |
|[GetStandardWidthInch](./getstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
|[SetStandardWidthInch](./setstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
|[GetStandardWidthPixels](./getstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
|[SetStandardWidthPixels](./setstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
|[GetStandardWidth](./getstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
|[SetStandardWidth](./setstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
|[GetStandardHeight](./getstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
|[SetStandardHeight](./setstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
|[GetStandardHeightPixels](./getstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
|[SetStandardHeightPixels](./setstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
|[GetStandardHeightInch](./getstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
|[SetStandardHeightInch](./setstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
|[ImportFormulaArray](./importformulaarray/) | Imports an array of formula into a worksheet. |
|[TextToColumns](./texttocolumns/) | Splits content in specified column into multiple columns.. |
|[ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Import a CSV file to the cells. |
|[ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Import a CSV file to the cells. |
|[ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Import a CSV file to the cells. |
|[ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Import a CSV file to the cells. |
|[GetPreserveString](./getpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings.Default is false. |
|[SetPreserveString](./setpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings.Default is false. |
|[Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Merges a specified range of cells into a single cell. |
|[Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Merges a specified range of cells into a single cell. |
|[Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Merges a specified range of cells into a single cell. |
|[UnMerge](./unmerge/) | Unmerges a specified range of merged cells. |
|[ClearMergedCells](./clearmergedcells/) | Clears all merged ranges. |
|[HideRow](./hiderow/) | Hides a row. |
|[UnhideRow](./unhiderow/) | Unhides a row. |
|[HideRows](./hiderows/) | Hides multiple rows. |
|[UnhideRows](./unhiderows/) | Unhides the hidden rows. |
|[SetRowHeightPixel](./setrowheightpixel/) | Sets row height in unit of pixels. |
|[SetRowHeightInch](./setrowheightinch/) | Sets row height in unit of inches. |
|[SetRowHeight](./setrowheight/) | Sets the height of the specified row. |
|[GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Gets row's height. |
|[GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Gets the column width. |
|[HideColumn](./hidecolumn/) | Hides a column. |
|[UnhideColumn](./unhidecolumn/) | Unhides a column |
|[HideColumns](./hidecolumns/) | Hide multiple columns. |
|[UnhideColumns](./unhidecolumns/) | Unhide multiple columns. |
|[GetRowHeight_Int](./getrowheight_int/) | Gets the height of a specified row, in unit of points. |
|[GetViewRowHeight](./getviewrowheight/) | Gets the height of a specified row. |
|[GetRowHeightInch](./getrowheightinch/) | Gets the height of a specified row in unit of inches. |
|[GetViewRowHeightInch](./getviewrowheightinch/) | Gets the height of a specified row in unit of inches. |
|[GetRowHeightPixel](./getrowheightpixel/) | Gets the height of a specified row in unit of pixel. |
|[SetColumnWidthPixel](./setcolumnwidthpixel/) | Sets column width in unit of pixels in normal view. |
|[SetColumnWidthInch](./setcolumnwidthinch/) | Sets column width in unit of inches  in normal view. |
|[SetColumnWidth](./setcolumnwidth/) | Sets the width of the specified column in normal view. |
|[GetColumnWidthPixel](./getcolumnwidthpixel/) | Gets the width of the specified column in normal view, in units of pixel. |
|[GetColumnWidth_Int](./getcolumnwidth_int/) | Gets the width(in unit of characters) of the specified column in normal view |
|[GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Get the width in different view type. |
|[SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Sets the width of the column in different view. |
|[GetMinRow](./getminrow/) | Minimum row index of cell which contains data or style. |
|[GetMaxRow](./getmaxrow/) | Maximum row index of cell which contains data or style. |
|[GetMinColumn](./getmincolumn/) | Minimum column index of those cells that have been instantiated in the collection(does not include the columnwhere style is defined for the whole column but no cell has been instantiated in it). |
|[GetMaxColumn](./getmaxcolumn/) | Maximum column index of those cells that have been instantiated in the collection(does not include the columnwhere style is defined for the whole column but no cell has been instantiated in it). |
|[GetMinDataRow](./getmindatarow/) | Minimum row index of cell which contains data. |
|[GetMaxDataRow](./getmaxdatarow/) | Maximum row index of cell which contains data. |
|[GetMinDataColumn](./getmindatacolumn/) | Minimum column index of cell which contains data. |
|[GetMaxDataColumn](./getmaxdatacolumn/) | Maximum column index of cell which contains data. |
|[GetLastDataRow](./getlastdatarow/) | Gets the last row index of cell which contains data in the specified column. |
|[GetFirstDataRow](./getfirstdatarow/) | Gets the first row index of cell which contains data in the specified column. |
|[IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Indicates that row height and default font height matches |
|[SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Indicates that row height and default font height matches |
|[IsDefaultRowHidden](./isdefaultrowhidden/) | Indicates whether the row is default hidden. |
|[SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Indicates whether the row is default hidden. |
|[GetColumns](./getcolumns/) | Gets the collection of Column objects that represents the individual columns in this worksheet. |
|[ApplyColumnStyle](./applycolumnstyle/) | Applies formats for a whole column. |
|[ApplyRowStyle](./applyrowstyle/) | Applies formats for a whole row. |
|[ApplyStyle](./applystyle/) | Applies formats for a whole worksheet. |
|[CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Copies data and formats of a whole column. |
|[CopyColumn](./copycolumn/) | Copies data and formats of a whole column. |
|[CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Copies data and formats of a whole column. |
|[CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Copies data and formats of the whole columns. |
|[CopyRow](./copyrow/) | Copies data and formats of a whole row. |
|[CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Copies data and formats of some whole rows. |
|[CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Copies data and formats of some whole rows. |
|[CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Copies data and formats of some whole rows. |
|[GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Gets the outline level (zero-based) of the row. |
|[GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Gets the outline level (zero-based) of the column. |
|[GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Gets the max grouped column outline level (zero-based). |
|[GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Gets the max grouped row outline level (zero-based). |
|[ShowGroupDetail](./showgroupdetail/) | Expands the grouped rows/columns. |
|[HideGroupDetail](./hidegroupdetail/) | Collapses the grouped rows/columns. |
|[UngroupColumns](./ungroupcolumns/) | Ungroups columns. |
|[GroupColumns_Int_Int](./groupcolumns_int_int/) | Groups columns. |
|[GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Groups columns. |
|[UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Ungroups rows. |
|[UngroupRows_Int_Int](./ungrouprows_int_int/) | Ungroups rows. |
|[GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Groups rows. |
|[GroupRows_Int_Int](./grouprows_int_int/) | Groups rows. |
|[DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Deletes a column. |
|[DeleteColumn_Int](./deletecolumn_int/) | Deletes a column. |
|[DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Deletes several columns. |
|[DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Deletes several columns. |
|[IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Check whether the range could be deleted. |
|[DeleteRow_Int](./deleterow_int/) | Deletes a row. |
|[DeleteRow_Int_Bool](./deleterow_int_bool/) | Deletes a row. |
|[DeleteRows_Int_Int](./deleterows_int_int/) | Deletes multiple rows. |
|[DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Deletes multiple rows in the worksheet. |
|[DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Deletes multiple rows in the worksheet. |
|[DeleteBlankColumns](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. |
|[DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Delete all blank columns which do not contain any data. |
|[IsBlankColumn](./isblankcolumn/) | Checks whether given column is blank(does not contain any data). |
|[DeleteBlankRows](./deleteblankrows/) | Delete all blank rows which do not contain any data or other object. |
|[DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
|[InsertColumns_Int_Int](./insertcolumns_int_int/) | Inserts some columns into the worksheet. |
|[InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Inserts some columns into the worksheet. |
|[InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Inserts some columns into the worksheet. |
|[InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Inserts a new column into the worksheet. |
|[InsertColumn_Int](./insertcolumn_int/) | Inserts a new column into the worksheet. |
|[InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Inserts multiple rows into the worksheet. |
|[InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Inserts multiple rows into the worksheet. |
|[InsertRows_Int_Int](./insertrows_int_int/) | Inserts multiple rows into the worksheet. |
|[InsertRow](./insertrow/) | Inserts a new row into the worksheet. |
|[GetRanges](./getranges/) | Gets the collection of Range objects created at run time. |
|[ClearRange_CellArea](./clearrange_cellarea/) | Clears contents and formatting of a range. |
|[ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Clears contents and formatting of a range. |
|[ClearContents_CellArea](./clearcontents_cellarea/) | Clears contents of a range. |
|[ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Clears contents of a range. |
|[ClearFormats_CellArea](./clearformats_cellarea/) | Clears formatting of a range. |
|[ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Clears formatting of a range. |
|[GetLastCell](./getlastcell/) | Gets the last cell in this worksheet. |
|[LinkToXmlMap](./linktoxmlmap/) | Link to a xml map. |
|[GetMaxDisplayRange](./getmaxdisplayrange/) | Gets the max range which includes data, merged cells and shapes. |
|[GetFirstCell](./getfirstcell/) | Gets the first cell in this worksheet. |
|[Find_Object_Cell](./find_object_cell/) | Finds the cell containing with the input object. |
|[Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Finds the cell containing with the input object. |
|[EndCellInRow_Int](./endcellinrow_int/) | Gets the last cell in this row. |
|[EndCellInColumn_Int](./endcellincolumn_int/) | Gets the last cell in this column. |
|[EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Gets the last cell with maximum column index in this range. |
|[EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Gets the last cell with maximum row index in this range. |
|[MoveRange](./moverange/) | Moves the range. |
|[InsertCutCells](./insertcutcells/) | Insert cut range. |
|[InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Inserts a range of cells and shift cells according to the shift option. |
|[InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Inserts a range of cells and shift cells according to the shift option. |
|[InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Inserts a range of cells and shift cells according to the shift option. |
|[DeleteRange](./deleterange/) | Deletes a range of cells and shift cells according to the shift option. |
|[ExportArray](./exportarray/) | Exports data in the Cells collection to a two-dimension array object. |
|[RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Retrieves subtotals setting of the range. |
|[Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Creates subtotals for the range. |
|[Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Creates subtotals for the range. |
|[RemoveFormulas](./removeformulas/) | Removes all formula and replaces with the value of the formula. |
|[RemoveDuplicates](./removeduplicates/) | Removes duplicate rows in the sheet. |
|[RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Removes duplicate values in the range. |
|[RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Removes duplicate data of the range. |
|[ConvertStringToNumericValue](./convertstringtonumericvalue/) | Converts all string data in the worksheet to numeric value if possible. |
|[GetDependents](./getdependents/) | Get all cells which refer to the specific cell. |
|[GetDependentsInCalculation](./getdependentsincalculation/) | Gets all cells whose calculated result depends on specific cell. |
|[GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Gets all cells that contain embedded picture. |
|[GetCellStyle](./getcellstyle/) | Get the style of given cell. |
|[GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Get the display style of given cell. |
|[GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Get the display style of given cell. |
