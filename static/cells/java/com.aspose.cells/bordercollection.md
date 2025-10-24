##BorderCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class BorderCollection
```
Encapsulates a collection of [Border](../../com.aspose.cells/border) objects.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(0);
//Accessing the "A1" cell from the worksheet
Cell cell = worksheet.getCells().get("A1");
//Adding some value to the "A1" cell
cell.putValue("Visit Aspose!");
Style style = cell.getStyle();
//Setting the line style of the top border
style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
//Setting the color of the top border
style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
//Setting the line style of the bottom border
style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
//Setting the color of the bottom border
style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
//Setting the line style of the left border
style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
//Setting the color of the left border
style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
//Setting the line style of the right border
style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
//Setting the color of the right border
style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
cell.setStyle(style);
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Gets the [Border](../../com.aspose.cells/border) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Gets the [Color](../../com.aspose.cells/color) of Diagonal lines. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Gets the style of Diagonal lines. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Sets the [Color](../../com.aspose.cells/color) of all borders in the collection. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Sets the [Color](../../com.aspose.cells/color) of Diagonal lines. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Sets the style of Diagonal lines. |
| [setStyle(int style)](#setStyle-int-) | Sets the style of all borders of the collection. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```
Gets the [Border](../../com.aspose.cells/border) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). The border to be retrieved. |
**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```
Gets the [Color](../../com.aspose.cells/color) of Diagonal lines.
**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```
Gets the style of Diagonal lines.
See [CellBorderType](../../com.aspose.cells/cellbordertype).
**Returns:**
int
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
### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```
Sets the [Color](../../com.aspose.cells/color) of all borders in the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Borders' [Color](../../com.aspose.cells/color). |
### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```
Sets the [Color](../../com.aspose.cells/color) of Diagonal lines.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```
Sets the style of Diagonal lines.
See [CellBorderType](../../com.aspose.cells/cellbordertype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```
Sets the style of all borders of the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borders' style |
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
