##Column
Represents a single column in a worksheet.
**Inheritance:**
java.lang.Object
```
public class Column
```
Represents a single column in a worksheet.
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
//Get first Column
Column column = worksheet.getCells().getColumns().get(0);
//Apply Style to first Column
column.applyStyle(style, styleFlag);
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole column. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Gets the group level of the column. |
| [getIndex()](#getIndex--) | Gets the index of this column. |
| [getStyle()](#getStyle--) | Gets the style of this column. |
| [getWidth()](#getWidth--) | Gets the column width in unit of characters. |
| [hasCustomStyle()](#hasCustomStyle--) | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | whether the column is collapsed |
| [isHidden()](#isHidden--) | Indicates whether the column is hidden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | whether the column is collapsed |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Gets the group level of the column. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the column is hidden. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Sets the style of this column. |
| [setWidth(double value)](#setWidth-double-) | Sets the column width in unit of characters. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```
Applies formats for a whole column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```
Gets the group level of the column.
**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the index of this column.
**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```
Gets the style of this column.
**Remarks**
Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) or [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) method to apply the change to this column.
Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```
Gets the column width in unit of characters.
**Remarks**
For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```
Indicates whether this column has custom style settings(different from the default one inherited from workbook).
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```
whether the column is collapsed
**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```
Indicates whether the column is hidden.
**Returns:**
boolean
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
whether the column is collapsed
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```
Gets the group level of the column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |
### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```
Indicates whether the column is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```
Sets the style of this column.
**Remarks**
This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | the style to be used as the default style for cells in this column. |
### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```
Sets the column width in unit of characters.
**Remarks**
For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
