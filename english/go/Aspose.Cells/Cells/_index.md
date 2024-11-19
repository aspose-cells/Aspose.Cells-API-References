---
title: Cells Class 
linktitle: Cells
second_title: Aspose.Cells for Go API Reference
description: 'Cells class. Encapsulates the object that represents cells in Go.'
type: docs
weight: 200
url: /go/aspose.cells/cells/
---

## Cells class

Encapsulates a collection of cell relevant objects, such as <see cref="Cell"/>, <see cref="Row"/>, ...etc.

```go

type Cells struct 

cells, _ := asposecells.NewCells()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewCells](./newcells/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetOdsCellFields](./getodscellfields/) | Gets the list of fields of ods. | 
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. | 
|[GetCount](./getcount/) | Gets the total count of instantiated Cell objects. | 
|[GetCountLarge](./getcountlarge/) | Gets the total count of instantiated Cell objects. | 
|[GetRows](./getrows/) | Gets the collection of <see cref="Row"/> objects that represents the individual rows in this worksheet. | 
|[CheckCell](./checkcell/) | Gets the <see cref="Cell"/> element or null at the specified cell row index and column index. | 
|[CheckRow](./checkrow/) | Gets the <see cref="Row"/> element or null at the specified cell row index. | 
|[CheckColumn](./checkcolumn/) | Gets the <see cref="Column"/> element or null at the specified column index. | 
|[IsRowHidden](./isrowhidden/) | Checks whether a row at given index is hidden. | 
|[IsColumnHidden](./iscolumnhidden/) | Checks whether a column at given index is hidden. | 
|[AddRange](./addrange/) | Adds a range object reference to cells | 
|[CreateRange](./createrange/) | Creates a <see cref="Range"/> object from a range of cells. | 
|[CreateRange](./createrange/) | Creates a <see cref="Range"/> object from a range of cells. | 
|[CreateRange](./createrange/) | Creates a <see cref="Range"/> object from an address of the range. | 
|[CreateRange](./createrange/) | Creates a <see cref="Range"/> object from rows of cells or columns of cells. | 
|[Get](./get/) | Gets the <see cref="Cell"/> element at the specified cell row index and column index. | 
|[Get](./get/) | Gets the <see cref="Cell"/> element at the specified cell name. | 
|[GetMultiThreadReading](./getmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading.Default value of this property is false. | 
|[SetMultiThreadReading](./setmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading.Default value of this property is false. | 
|[GetMemorySetting](./getmemorysetting/) | Gets or sets the memory usage option for this cells. | 
|[SetMemorySetting](./setmemorysetting/) | Gets or sets the memory usage option for this cells. | 
|[Clear](./clear/) | Clears all data of the worksheet. | 
|[GetStyle](./getstyle/) | Gets and sets the default style of the worksheet. | 
|[SetStyle](./setstyle/) | Gets and sets the default style of the worksheet. | 
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
|[TextToColumns](./texttocolumns/) | Splits content in specified column into multiple columns.. | 
|[ImportCSV](./importcsv/) | Import a CSV file to the cells. | 
|[ImportCSV](./importcsv/) | Import a CSV file to the cells. | 
|[GetPreserveString](./getpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings.Default is false. | 
|[SetPreserveString](./setpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings.Default is false. | 
|[Merge](./merge/) | Merges a specified range of cells into a single cell. | 
|[Merge](./merge/) | Merges a specified range of cells into a single cell. | 
|[Merge](./merge/) | Merges a specified range of cells into a single cell. | 
|[UnMerge](./unmerge/) | Unmerges a specified range of merged cells. | 
|[ClearMergedCells](./clearmergedcells/) | Clears all merged ranges. | 
|[HideRow](./hiderow/) | Hides a row. | 
|[UnhideRow](./unhiderow/) | Unhides a row. | 
|[HideRows](./hiderows/) | Hides multiple rows. | 
|[UnhideRows](./unhiderows/) | Unhides the hidden rows. | 
|[SetRowHeightPixel](./setrowheightpixel/) | Sets row height in unit of pixels. | 
|[SetRowHeightInch](./setrowheightinch/) | Sets row height in unit of inches. | 
|[SetRowHeight](./setrowheight/) | Sets the height of the specified row. | 
|[GetRowHeight](./getrowheight/) | Gets row's height. | 
|[GetColumnWidth](./getcolumnwidth/) | Gets the column width. | 
|[HideColumn](./hidecolumn/) | Hides a column. | 
|[UnhideColumn](./unhidecolumn/) | Unhides a column | 
|[HideColumns](./hidecolumns/) | Hide multiple columns. | 
|[UnhideColumns](./unhidecolumns/) | Unhide multiple columns. | 
|[GetRowHeight](./getrowheight/) | Gets the height of a specified row, in unit of points. | 
|[GetViewRowHeight](./getviewrowheight/) | Gets the height of a specified row. | 
|[GetRowHeightInch](./getrowheightinch/) | Gets the height of a specified row in unit of inches. | 
|[GetViewRowHeightInch](./getviewrowheightinch/) | Gets the height of a specified row in unit of inches. | 
|[GetRowHeightPixel](./getrowheightpixel/) | Gets the height of a specified row in unit of pixel. | 
|[SetColumnWidthPixel](./setcolumnwidthpixel/) | Sets column width in unit of pixels in normal view. | 
|[SetColumnWidthInch](./setcolumnwidthinch/) | Sets column width in unit of inches  in normal view. | 
|[SetColumnWidth](./setcolumnwidth/) | Sets the width of the specified column in normal view. | 
|[GetColumnWidthPixel](./getcolumnwidthpixel/) | Gets the width of the specified column in normal view, in units of pixel. | 
|[GetColumnWidth](./getcolumnwidth/) | Gets the width(in unit of characters) of the specified column in normal view | 
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
|[IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Indicates that row height and default font height matches | 
|[SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Indicates that row height and default font height matches | 
|[IsDefaultRowHidden](./isdefaultrowhidden/) | Indicates whether the row is default hidden. | 
|[SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Indicates whether the row is default hidden. | 
|[GetColumns](./getcolumns/) | Gets the collection of <see cref="Column"/> objects that represents the individual columns in this worksheet. | 
|[ApplyColumnStyle](./applycolumnstyle/) | Applies formats for a whole column. | 
|[ApplyRowStyle](./applyrowstyle/) | Applies formats for a whole row. | 
|[ApplyStyle](./applystyle/) | Applies formats for a whole worksheet. | 
|[CopyColumns](./copycolumns/) | Copies data and formats of a whole column. | 
|[CopyColumn](./copycolumn/) | Copies data and formats of a whole column. | 
|[CopyColumns](./copycolumns/) | Copies data and formats of a whole column. | 
|[CopyColumns](./copycolumns/) | Copies data and formats of the whole columns. | 
|[CopyRow](./copyrow/) | Copies data and formats of a whole row. | 
|[CopyRows](./copyrows/) | Copies data and formats of some whole rows. | 
|[CopyRows](./copyrows/) | Copies data and formats of some whole rows. | 
|[CopyRows](./copyrows/) | Copies data and formats of some whole rows. | 
|[GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Gets the outline level (zero-based) of the row. | 
|[GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Gets the outline level (zero-based) of the column. | 
|[GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Gets the max grouped column outline level (zero-based). | 
|[GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Gets the max grouped row outline level (zero-based). | 
|[ShowGroupDetail](./showgroupdetail/) | Expands the grouped rows/columns. | 
|[HideGroupDetail](./hidegroupdetail/) | Collapses the grouped rows/columns. | 
|[UngroupColumns](./ungroupcolumns/) | Ungroups columns. | 
|[GroupColumns](./groupcolumns/) | Groups columns. | 
|[GroupColumns](./groupcolumns/) | Groups columns. | 
|[UngroupRows](./ungrouprows/) | Ungroups rows. | 
|[UngroupRows](./ungrouprows/) | Ungroups rows. | 
|[GroupRows](./grouprows/) | Groups rows. | 
|[GroupRows](./grouprows/) | Groups rows. | 
|[DeleteColumn](./deletecolumn/) | Deletes a column. | 
|[DeleteColumn](./deletecolumn/) | Deletes a column. | 
|[DeleteColumns](./deletecolumns/) | Deletes several columns. | 
|[IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Check whether the range could be deleted. | 
|[DeleteRow](./deleterow/) | Deletes a row. | 
|[DeleteRows](./deleterows/) | Deletes several rows. | 
|[DeleteRow](./deleterow/) | Deletes a row. | 
|[DeleteRows](./deleterows/) | Deletes multiple rows in the worksheet. | 
|[DeleteBlankColumns](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. | 
|[DeleteBlankColumns](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. | 
|[IsBlankColumn](./isblankcolumn/) | Checks whether given column is blank(does not contain any data). | 
|[DeleteBlankRows](./deleteblankrows/) | Delete all blank rows which do not contain any data or other object. | 
|[DeleteBlankRows](./deleteblankrows/) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. | 
|[InsertColumns](./insertcolumns/) | Inserts some columns into the worksheet. | 
|[InsertColumns](./insertcolumns/) | Inserts some columns into the worksheet. | 
|[InsertColumn](./insertcolumn/) | Inserts a new column into the worksheet. | 
|[InsertColumn](./insertcolumn/) | Inserts a new column into the worksheet. | 
|[InsertRows](./insertrows/) | Inserts multiple rows into the worksheet. | 
|[InsertRows](./insertrows/) | Inserts multiple rows into the worksheet. | 
|[InsertRows](./insertrows/) | Inserts multiple rows into the worksheet. | 
|[InsertRow](./insertrow/) | Inserts a new row into the worksheet. | 
|[GetRanges](./getranges/) | Gets the collection of <see cref="Range"/> objects created at run time. | 
|[ClearRange](./clearrange/) | Clears contents and formatting of a range. | 
|[ClearRange](./clearrange/) | Clears contents and formatting of a range. | 
|[ClearContents](./clearcontents/) | Clears contents of a range. | 
|[ClearContents](./clearcontents/) | Clears contents of a range. | 
|[ClearFormats](./clearformats/) | Clears formatting of a range. | 
|[ClearFormats](./clearformats/) | Clears formatting of a range. | 
|[GetLastCell](./getlastcell/) | Gets the last cell in this worksheet. | 
|[LinkToXmlMap](./linktoxmlmap/) | Link to a xml map. | 
|[GetMaxDisplayRange](./getmaxdisplayrange/) | Gets the max range which includes data, merged cells and shapes. | 
|[GetFirstCell](./getfirstcell/) | Gets the first cell in this worksheet. | 
|[Find](./find/) | Finds the cell containing with the input object. | 
|[Find](./find/) | Finds the cell containing with the input object. | 
|[EndCellInRow](./endcellinrow/) | Gets the last cell in this row. | 
|[EndCellInColumn](./endcellincolumn/) | Gets the last cell in this column. | 
|[EndCellInColumn](./endcellincolumn/) | Gets the last cell with maximum column index in this range. | 
|[EndCellInRow](./endcellinrow/) | Gets the last cell with maximum row index in this range. | 
|[MoveRange](./moverange/) | Moves the range. | 
|[InsertCutCells](./insertcutcells/) | Insert cut range. | 
|[InsertRange](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. | 
|[InsertRange](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. | 
|[InsertRange](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. | 
|[DeleteRange](./deleterange/) | Deletes a range of cells and shift cells according to the shift option. | 
|[RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Retrieves subtotals setting of the range. | 
|[RemoveFormulas](./removeformulas/) | Removes all formula and replaces with the value of the formula. | 
|[RemoveDuplicates](./removeduplicates/) | Removes duplicate rows in the sheet. | 
|[RemoveDuplicates](./removeduplicates/) | Removes duplicate values in the range. | 
|[ConvertStringToNumericValue](./convertstringtonumericvalue/) | Converts all string data in the worksheet to numeric value if possible. | 
|[GetCellStyle](./getcellstyle/) | Get the style of given cell. | 
