##Row
Represents a single row in a worksheet.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```
Represents a single row in a worksheet.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
Style style = workbook.createStyle();
//Setting the background color to Blue
style.setBackgroundColor(Color.getBlue());
//Setting the foreground color to Red
style.setForegroundColor(Color.getRed());
//setting Background Pattern
style.setPattern(BackgroundType.DIAGONAL_STRIPE);
//New Style Flag
StyleFlag styleFlag = new StyleFlag();
//Set All Styles
styleFlag.setAll(true);
//Get first row
Row row = worksheet.getCells().getRows().get(0);
//Apply Style to first row
row.applyStyle(style, styleFlag);
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole row. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Copy settings of row, such as style, height, visibility, ...etc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Checks whether this object refers to the same row with another row object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Checks whether this object refers to the same row with another. |
| [get(int column)](#get-int-) | Gets the cell. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Get the cell by specific index in the cells collection of this row. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Gets the cell or null in the specific index. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Gets the first cell object in the row. |
| [getFirstDataCell()](#getFirstDataCell--) | Gets the first non-blank cell in the row. |
| [getGroupLevel()](#getGroupLevel--) | Gets the group level of the row. |
| [getHeight()](#getHeight--) | Gets the row height in unit of Points. |
| [getIndex()](#getIndex--) | Gets the index of this row. |
| [getLastCell()](#getLastCell--) | Gets the last cell object in the row. |
| [getLastDataCell()](#getLastDataCell--) | Gets the last non-blank cell in the row. |
| [getStyle()](#getStyle--) | Gets the style of this row. |
| [hasCustomStyle()](#hasCustomStyle--) | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indicates whether the row contains any data |
| [isCollapsed()](#isCollapsed--) | whether the row is collapsed |
| [isHeightMatched()](#isHeightMatched--) | Indicates whether the row height matches current default font setting of the workbook. |
| [isHidden()](#isHidden--) | Indicates whether the row is hidden. |
| [iterator()](#iterator--) | Gets the cells enumerator |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Gets an enumerator that iterates cells through this row. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | whether the row is collapsed |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Gets the group level of the row. |
| [setHeight(double value)](#setHeight-double-) | Sets the row height in unit of Points. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Indicates whether the row height matches current default font setting of the workbook. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the row is hidden. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Sets the style of this row. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```
Applies formats for a whole row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |
### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```
Copy settings of row, such as style, height, visibility, ...etc.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | the source row whose settings will be copied to this one |
| checkStyle | boolean | whether check and gather style. Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |
### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```
Checks whether this object refers to the same row with another row object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | another row object |
**Returns:**
boolean - true if two row objects refers to the same row.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Checks whether this object refers to the same row with another.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | another object |
**Returns:**
boolean - true if two objects refers to the same row.
### get(int column) {#get-int-}
```
public Cell get(int column)
```
Gets the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index |
**Returns:**
[Cell](../../com.aspose.cells/cell) -
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```
Get the cell by specific index in the cells collection of this row.
**Remarks**
To traverse all cells in sequence without modification, using [iterator()](../../com.aspose.cells/row\#iterator--) will give better performance than using this method to get cell one by one.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index(position) of the cell in the cells collection of this row. |
**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```
Gets the cell or null in the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index |
**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```
Gets the first cell object in the row.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```
Gets the first non-blank cell in the row.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```
Gets the group level of the row.
**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```
Gets the row height in unit of Points.
**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the index of this row.
**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```
Gets the last cell object in the row.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```
Gets the last non-blank cell in the row.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```
Gets the style of this row.
**Remarks**
Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call [Column.applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) or [Column.setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) method to apply the change to this row.
Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```
Indicates whether this row has custom style settings(different from the default one inherited from workbook).
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```
Indicates whether the row contains any data
**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```
whether the row is collapsed
**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
**Remarks**
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) to get the same result with what is shown in ms excel when you opening the workbook in it.
**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```
Indicates whether the row is hidden.
**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the cells enumerator
**Example**
```
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.getWorksheets().get(0).getCells();
Iterator en = cells.getRows().get(1).iterator();
while (en.hasNext())
{
Cell cell = (Cell)en.next();
System.out.println(cell.getName() + ": " + cell.getValue());
}
```
**Returns:**
java.util.Iterator - The cells enumerator which will traverse all existing cells in this row.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```
Gets an enumerator that iterates cells through this row.
**Remarks**
If the row will be modified(by operations that may cause new Cell be instantiated or existing Cell be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | boolean | whether enumerate cells in reversed order |
| sync | boolean | whether the returned enumerator should check the modification of cells in this row and keep synchronized with it. |
**Returns:**
java.util.Iterator - The cells enumerator which will traverse all existing cells in this row.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```
whether the row is collapsed
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```
Gets the group level of the row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |
### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```
Sets the row height in unit of Points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
**Remarks**
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) to get the same result with what is shown in ms excel when you opening the workbook in it.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```
Indicates whether the row is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```
Sets the style of this row.
**Remarks**
This method only sets the given style as the default style for this row, without changing the style settings for existing cells in this row. To update style settings of existing cells to the specified style at the same time, please use [Column.applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | the style to be used as the default style for cells in this row. |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
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
