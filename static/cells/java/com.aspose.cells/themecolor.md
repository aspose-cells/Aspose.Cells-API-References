##ThemeColor
Represents a theme color.
**Inheritance:**
java.lang.Object
```
public class ThemeColor
```
Represents a theme color.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Cells cells = workbook.getWorksheets().get(0).getCells();
cells.get("A1").putValue("Hello World");
Style style = cells.get("A1").getStyle();
//Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.getFont().setThemeColor(new ThemeColor(ThemeColorType.TEXT_2, 0.4));
style.setPattern(BackgroundType.SOLID);
//Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.setForegroundThemeColor(new ThemeColor(ThemeColorType.BACKGROUND_2, -0.75));
cells.get("A1").setStyle(style);
//Saving the Excel file
workbook.save("book1.xlsx");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | Gets the theme type. |
| [getTint()](#getTint--) | Gets the tint value. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | Sets the theme type. |
| [setTint(double value)](#setTint-double-) | Sets the tint value. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). The theme type. |
| tint | double | The tint value. |
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
### getColorType() {#getColorType--}
```
public int getColorType()
```
Gets the theme type.
See [ThemeColorType](../../com.aspose.cells/themecolortype).
**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```
Gets the tint value.
**Remarks**
The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.
**Returns:**
double
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
### setColorType(int value) {#setColorType-int-}
```
public void setColorType(int value)
```
Sets the theme type.
See [ThemeColorType](../../com.aspose.cells/themecolortype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```
Sets the tint value.
**Remarks**
The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.
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
