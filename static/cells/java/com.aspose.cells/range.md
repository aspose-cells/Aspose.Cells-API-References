##Range
Encapsulates the object that represents a range of cells within a spreadsheet.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```
Encapsulates the object that represents a range of cells within a spreadsheet.
**Remarks**
The Range class denotes a region of Excel spreadsheet. With this, you can format and set value of the range. And you can simply copy range of Excel too.
**Example**
The following example shows how to create a range and set value the range of Excel.
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.getWorksheets().get(0).getCells();
// Create a range (A1:D3).
Range range = cells.createRange("A1", "D3");
// Set value to the range.
range.setValue("Hello");
//Save the Excel file
workbook.save("book1.xlsm");
```
## Methods
| Method | Description |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole range. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Automaticall fill the target range. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Automaticall fill the target range. |
| [clear()](#clear--) | Clears this range. |
| [clearComments()](#clearComments--) | Clears the comments of this range. |
| [clearContents()](#clearContents--) | Clears the contents of this range. |
| [clearFormats()](#clearFormats--) | Clears the formats of this range. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Only removes hyperlinks. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Copying the range with paste special options. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Copies cell data (including formulas) from a source range. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Copies style settings from a source range. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Copies cell value from a source range. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Gets [Cell](../../com.aspose.cells/cell) object in this range. |
| [getAddress()](#getAddress--) | Gets address of the range. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Gets [Cell](../../com.aspose.cells/cell) object or null in this range. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Gets the count of columns in the range. |
| [getColumnWidth()](#getColumnWidth--) | Sets or gets the column width of this range |
| [getCurrentRegion()](#getCurrentRegion--) | Returns a Range object that represents the current region. |
| [getEntireColumn()](#getEntireColumn--) | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [getEntireRow()](#getEntireRow--) | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [getFirstColumn()](#getFirstColumn--) | Gets the index of the first column of the range. |
| [getFirstRow()](#getFirstRow--) | Gets the index of the first row of the range. |
| [getHeight()](#getHeight--) | Gets the width of a range in points. |
| [getHyperlinks()](#getHyperlinks--) | Gets all hyperlink in the range. |
| [getLeft()](#getLeft--) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [getName()](#getName--) | Gets the name of the range. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Gets [Range](../../com.aspose.cells/range) range by offset. |
| [getRefersTo()](#getRefersTo--) | Gets the range's refers to. |
| [getRowCount()](#getRowCount--) | Gets the count of rows in the range. |
| [getRowHeight()](#getRowHeight--) | Sets or gets the height of rows in this range |
| [getTop()](#getTop--) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [getValue()](#getValue--) | Gets the value of the range. |
| [getWidth()](#getWidth--) | Gets the width of a range in points. |
| [getWorksheet()](#getWorksheet--) | Gets the [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)object which contains this range. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Returns a [Range](../../com.aspose.cells/range) object that represents the rectangular intersection of two ranges. |
| [isBlank()](#isBlank--) | Indicates whether the range contains values. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Indicates whether the range is intersect. |
| [iterator()](#iterator--) | Gets the enumerator for cells in this Range. |
| [merge()](#merge--) | Combines a range of cells into a single cell. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Move the current range to the dest range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Sets or gets the column width of this range |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Set inside borders of the range. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the range. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Sets outline border around a range of cells. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Sets outline border around a range of cells. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Sets out line borders around a range of cells. |
| [setRowHeight(double value)](#setRowHeight-double-) | Sets or gets the height of rows in this range |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Sets the style of the range. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Apply the cell style. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sets the value of the range. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Convert the range to html . |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Converts the range to image. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Convert the range to JSON value. |
| [toString()](#toString--) | Returns a string represents the current Range object. |
| [transpose()](#transpose--) | Transpose (rotate) data from rows to columns or vice versa. |
| [unMerge()](#unMerge--) | Unmerges merged cells of this range. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Returns the union of two ranges. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Returns the union result of two ranges. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Returns the union result of two ranges. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | Address of the hyperlink. |
| textToDisplay | java.lang.String | The text to be displayed for the specified hyperlink. |
| screenTip | java.lang.String | The screenTip text for the specified hyperlink. |
**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```
Applies formats for a whole range.
**Remarks**
Each cell in this range will contains a [Style](../../com.aspose.cells/style) object. So this is a memory-consuming method. Please use it carefully.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |
### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```
Automaticall fill the target range.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.getWorksheets().get(0).getCells();
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
Range source = cells.createRange("A1:A2");
Range target = cells.createRange("A3:A10");
//fill 3,4,5....10 to the range A3:A10
source.autoFill(target);
//Save the Excel file
workbook.save("book1.xlsm");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | the target range. |
### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```
Automaticall fill the target range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | The targed range. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). The auto fill type. |
### clear() {#clear--}
```
public void clear()
```
Clears this range.
### clearComments() {#clearComments--}
```
public void clearComments()
```
Clears the comments of this range.
### clearContents() {#clearContents--}
```
public void clearContents()
```
Clears the contents of this range.
### clearFormats() {#clearFormats--}
```
public void clearFormats()
```
Clears the formats of this range.
### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```
Only removes hyperlinks.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| clearFormat | boolean | Indicates whether to clear the format of hyperlinks. |
### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```
Copies data (including formulas), formatting, drawing objects etc. from a source range.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.getWorksheets().get(0).getCells();
Range range1 = cells.createRange("A1:A5");
Range range2 = cells.createRange("A6:A10");
//Copy the range.
range1.copy(range2);
//Save the Excel file
workbook.save("book1.xlsm");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Source [Range](../../com.aspose.cells/range) object. |
### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```
Copying the range with paste special options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | The source range. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | The paste special options. |
### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```
Copies cell data (including formulas) from a source range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Source [Range](../../com.aspose.cells/range) object. |
### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```
Copies style settings from a source range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Source [Range](../../com.aspose.cells/range) object. |
### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```
Copies cell value from a source range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Source [Range](../../com.aspose.cells/range) object. |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```
Gets [Cell](../../com.aspose.cells/cell) object in this range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Row offset in this range, zero based. |
| columnOffset | int | Column offset in this range, zero based. |
**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```
Gets address of the range.
**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```
Gets [Cell](../../com.aspose.cells/cell) object or null in this range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Row offset in this range, zero based. |
| columnOffset | int | Column offset in this range, zero based. |
**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```
Gets the count of columns in the range.
**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```
Sets or gets the column width of this range
**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```
Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns.
**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```
Gets a Range object that represents the entire column (or columns) that contains the specified range.
**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```
Gets a Range object that represents the entire row (or rows) that contains the specified range.
**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```
Gets the index of the first column of the range.
**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```
Gets the index of the first row of the range.
**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```
Gets the width of a range in points.
**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```
Gets all hyperlink in the range.
**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```
Gets the distance, in points, from the left edge of column A to the left edge of the range.
**Returns:**
double
### getName() {#getName--}
```
public String getName()
```
Gets the name of the range.
**Remarks**
Named range is supported. For example,
range.Name = "Sheet1!MyRange";
**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```
Gets [Range](../../com.aspose.cells/range) range by offset.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Row offset in this range, zero based. |
| columnOffset | int | Column offset in this range, zero based. |
**Returns:**
[Range](../../com.aspose.cells/range) -
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```
Gets the range's refers to.
**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```
Gets the count of rows in the range.
**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```
Sets or gets the height of rows in this range
**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```
Gets the distance, in points, from the top edge of row 1 to the top edge of the range.
**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the value of the range.
**Remarks**
If the range contains multiple cells, the returned/applied object should be Object[][].
**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```
Gets the width of a range in points.
**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```
Gets the [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)object which contains this range.
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```
Returns a [Range](../../com.aspose.cells/range) object that represents the rectangular intersection of two ranges.
**Remarks**
If the two ranges are not intersected, returns null.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.getWorksheets().get(0).getCells();
Range range1 = cells.createRange("A1:A5");
Range range2 = cells.createRange("A3:A10");
//Get intersected range of the two ranges.
Range intersectRange = range1.intersect(range2);
//Save the Excel file
workbook.save("book1.xlsm");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | The intersecting range. |
**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```
Indicates whether the range contains values.
**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```
Indicates whether the range is intersect.
**Remarks**
If the two ranges area not in the same worksheet ,return false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | The range. |
**Returns:**
boolean - Whether the range is intersect.
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the enumerator for cells in this Range.
**Remarks**
When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
**Example**
```
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.getWorksheets().get(0).getCells();
Iterator en = cells.createRange("B2:C3").iterator();
while (en.hasNext())
{
Cell cell = (Cell)en.next();
System.out.println(cell.getName() + ": " + cell.getValue());
}
```
**Returns:**
java.util.Iterator - The cells enumerator
### merge() {#merge--}
```
public void merge()
```
Combines a range of cells into a single cell.
**Remarks**
Reference the merged cell via the address of the upper-left cell in the range.
### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```
Move the current range to the dest range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destRow | int | The start row of the dest range. |
| destColumn | int | The start column of the dest range. |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```
Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |
### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```
Sets or gets the column width of this range
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```
Set inside borders of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Inside borde type, only can be [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) and [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). The border style. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | The color of the border. |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the range.
**Remarks**
Named range is supported. For example,
range.Name = "Sheet1!MyRange";
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```
Sets outline border around a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Border edge. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Border style. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Border color. |
### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```
Sets outline border around a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Border edge. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Border style. |
| borderColor | [Color](../../com.aspose.cells/color) | Border color. |
### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```
Sets the outline borders around a range of cells with same border style and color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Border style. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Border color. |
### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```
Sets the outline borders around a range of cells with same border style and color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Border style. |
| borderColor | [Color](../../com.aspose.cells/color) | Border color. |
### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```
Sets out line borders around a range of cells.
**Remarks**
Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Border styles. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Border colors. |
### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```
Sets or gets the height of rows in this range
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```
Sets the style of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The Style object. |
### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```
Apply the cell style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Sets the value of the range.
**Remarks**
If the range contains multiple cells, the returned/applied object should be Object[][].
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```
Convert the range to html .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Options for coverting range to html. |
**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```
Converts the range to image.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | The options for converting this range to image |
**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```
Convert the range to JSON value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | The options of converting |
**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```
Returns a string represents the current Range object.
**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```
Transpose (rotate) data from rows to columns or vice versa.
### unMerge() {#unMerge--}
```
public void unMerge()
```
Unmerges merged cells of this range.
### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```
Returns the union of two ranges.
**Remarks**
NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | The range |
**Returns:**
java.util.ArrayList - The union of two ranges.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```
Returns the union result of two ranges.
**Remarks**
NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | The range |
**Returns:**
com.aspose.cells.Range[] - The union of two ranges.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```
Returns the union result of two ranges.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | The range |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
