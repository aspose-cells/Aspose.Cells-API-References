##UnionRange
Represents union range.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```
Represents union range.
## Methods
| Method | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole range. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Copying the range with paste special options. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Gets all cell count in the range. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Gets the count of rows in the range. |
| [getFirstColumn()](#getFirstColumn--) | Gets the index of the first column of the range. |
| [getFirstRow()](#getFirstRow--) | Gets the index of the first row of the range. |
| [getHyperlinks()](#getHyperlinks--) | Gets all hyperlink in the range. |
| [getName()](#getName--) | Gets the name of the range. |
| [getRangeCount()](#getRangeCount--) | Gets the count of the ranges. |
| [getRanges()](#getRanges--) | Gets all union ranges. |
| [getRefersTo()](#getRefersTo--) | Gets the range's refers to. |
| [getRowCount()](#getRowCount--) | Gets the count of rows in the range. |
| [getValue()](#getValue--) | Gets the values of the range. |
| [hasRange()](#hasRange--) | Indicates whether this has range. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Intersects another range. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Intersects another range. |
| [intersect(String range)](#intersect-java.lang.String-) | Intersects another range. |
| [iterator()](#iterator--) | Gets the enumerator for cells in this Range. |
| [merge()](#merge--) | Combines a range of cells into a single cell. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the range. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Sets out line borders around a range of cells. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Sets the style of the range. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sets the values of the range. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Unmerges merged cells of this range. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Union the ranges. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Union another range. |
| [union(String range)](#union-java.lang.String-) | Union another range. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```
Copying the range with paste special options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | The source range. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | The paste special options. |
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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```
Gets all cell count in the range.
**Returns:**
int
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
Gets the count of rows in the range.
**Remarks**
Only effects when it only contains one range.
**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```
Gets the index of the first column of the range.
**Remarks**
Only effects when it only contains one range.
**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```
Gets the index of the first row of the range.
**Remarks**
Only effects when it only contains one range.
**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```
Gets all hyperlink in the range.
**Returns:**
com.aspose.cells.Hyperlink[]
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
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```
Gets the count of the ranges.
**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```
Gets all union ranges.
**Returns:**
com.aspose.cells.Range[]
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
**Remarks**
Only effects when it only contains one range.
**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the values of the range.
**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```
Indicates whether this has range.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```
Intersects another range.
**Remarks**
If the two union ranges are not intersected, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | The range. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```
Intersects another range.
**Remarks**
If the two union ranges are not intersected, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | The range. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```
Intersects another range.
**Remarks**
If the two union ranges are not intersected, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | java.lang.String | The range. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the enumerator for cells in this Range.
**Remarks**
When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
**Returns:**
java.util.Iterator - The cells enumerator
### merge() {#merge--}
```
public void merge()
```
Combines a range of cells into a single cell.
**Remarks**
Reference the merged cell via the address of the upper-left cell in the range.
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
### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```
Sets the style of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The Style object. |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Sets the values of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```
Unmerges merged cells of this range.
### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```
Union the ranges.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | The ranges. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) -
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```
Union another range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | The range. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) -
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```
Union another range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | java.lang.String | The range. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) -
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
