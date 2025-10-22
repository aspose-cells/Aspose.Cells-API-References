##CellsColor
Represents all types of color.
**Inheritance:**
java.lang.Object
```
public class CellsColor
```
Represents all types of color.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Gets the color from a 32-bit ARGB value. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets the RGB color. |
| [getColorIndex()](#getColorIndex--) | Gets the color index in the color palette. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color. |
| [getTransparency()](#getTransparency--) | Gets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | The color type. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Gets the color which should apply to cell or shape. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Sets the color from a 32-bit ARGB value. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Sets the RGB color. |
| [setColorIndex(int value)](#setColorIndex-int-) | Sets the color index in the color palette. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Sets the color which should apply to cell or shape. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Gets the theme color. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Set the tint of the shape color |
| [setTransparency(double value)](#setTransparency-double-) | Sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```
Gets the color from a 32-bit ARGB value.
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
Gets the RGB color.
**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```
Gets the color index in the color palette. Only applies of indexed color.
**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```
Gets the theme color. Only applies for theme color type.
**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```
Gets transparency as a value from 0.0 (opaque) through 1.0 (clear).
**Returns:**
double
### getType() {#getType--}
```
public int getType()
```
The color type.
See [ColorType](../../com.aspose.cells/colortype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```
Gets the color which should apply to cell or shape.
**Remarks**
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
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
### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```
Sets the color from a 32-bit ARGB value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```
Sets the RGB color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```
Sets the color index in the color palette. Only applies of indexed color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```
Sets the color which should apply to cell or shape.
**Remarks**
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```
Gets the theme color. Only applies for theme color type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |
### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```
Set the tint of the shape color
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tint | double |  |
### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```
Sets transparency as a value from 0.0 (opaque) through 1.0 (clear).
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
