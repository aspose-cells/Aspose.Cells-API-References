##TextEffectFormat
Contains properties and methods that apply to WordArt objects.
**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```
Contains properties and methods that apply to WordArt objects.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
workbook.save("Book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Indicates whether font is bold. |
| [getFontItalic()](#getFontItalic--) | Indicates whether font is italic. |
| [getFontName()](#getFontName--) | The name of the font used in the WordArt. |
| [getFontSize()](#getFontSize--) | The size (in points) of the font used in the WordArt. |
| [getPresetShape()](#getPresetShape--) | Gets the preset shape type. |
| [getRotatedChars()](#getRotatedChars--) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [getText()](#getText--) | The text in the WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Indicates whether font is bold. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Indicates whether font is italic. |
| [setFontName(String value)](#setFontName-java.lang.String-) | The name of the font used in the WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | The size (in points) of the font used in the WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Sets the preset shape type. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [setText(String value)](#setText-java.lang.String-) | The text in the WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Sets the preset text effect. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```
Indicates whether font is bold.
**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```
Indicates whether font is italic.
**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```
The name of the font used in the WordArt.
**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```
The size (in points) of the font used in the WordArt.
**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```
Gets the preset shape type.
See [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).
**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```
If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape.
**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```
The text in the WordArt.
**Returns:**
java.lang.String
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
### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```
Indicates whether font is bold.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```
Indicates whether font is italic.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```
The name of the font used in the WordArt.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```
The size (in points) of the font used in the WordArt.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```
Sets the preset shape type.
See [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```
If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
The text in the WordArt.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```
Sets the preset text effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). The preset text effect. |
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
