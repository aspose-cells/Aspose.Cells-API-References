##Border
Encapsulates the object that represents the cell border.
**Inheritance:**
java.lang.Object
```
public class Border
```
Encapsulates the object that represents the cell border.
**Example**
```
Workbook workbook = new Workbook();
WorksheetCollection sheets = workbook.getWorksheets();
Cell cell = sheets.get(0).getCells().get("A1");
Style style = cell.getStyle();
//Set top border style and color
Border border = style.getBorders().getByBorderType(BorderType.TOP_BORDER);
border.setLineStyle(CellBorderType.MEDIUM);
border.setColor(Color.getRed());
cell.setStyle(style);
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Gets the color with a 32-bit ARGB value. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets the [Color](../../com.aspose.cells/color) of the border. |
| [getLineStyle()](#getLineStyle--) | Gets the cell border type. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color of the border. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Sets the color with a 32-bit ARGB value. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Sets the [Color](../../com.aspose.cells/color) of the border. |
| [setLineStyle(int value)](#setLineStyle-int-) | Sets the cell border type. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Sets the theme color of the border. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```
Gets the color with a 32-bit ARGB value.
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```
Gets the [Color](../../com.aspose.cells/color) of the border.
**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```
Gets the cell border type.
See [CellBorderType](../../com.aspose.cells/cellbordertype).
**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```
Gets the theme color of the border.
**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```
Sets the color with a 32-bit ARGB value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```
Sets the [Color](../../com.aspose.cells/color) of the border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```
Sets the cell border type.
See [CellBorderType](../../com.aspose.cells/cellbordertype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```
Sets the theme color of the border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |
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
