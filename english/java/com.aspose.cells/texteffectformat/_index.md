---
title: TextEffectFormat
second_title: Aspose.Cells for Java API Reference
description: Contains properties and methods that apply to WordArt objects.
type: docs
weight: 574
url: /java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Contains properties and methods that apply to WordArt objects.

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
| [getPresetShape()](#getPresetShape--) | Gets and sets the preset shape type. |
| [getRotatedChars()](#getRotatedChars--) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [getText()](#getText--) | The text in the WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Please see the getter of this property: [getFontBold()](../../com.aspose.cells/texteffectformat\#getFontBold--) |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Please see the getter of this property: [getFontItalic()](../../com.aspose.cells/texteffectformat\#getFontItalic--) |
| [setFontName(String value)](#setFontName-java.lang.String-) | Please see the getter of this property: [getFontName()](../../com.aspose.cells/texteffectformat\#getFontName--) |
| [setFontSize(int value)](#setFontSize-int-) | Please see the getter of this property: [getFontSize()](../../com.aspose.cells/texteffectformat\#getFontSize--) |
| [setPresetShape(int value)](#setPresetShape-int-) | Please see the getter of this property: [getPresetShape()](../../com.aspose.cells/texteffectformat\#getPresetShape--) |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Please see the getter of this property: [getRotatedChars()](../../com.aspose.cells/texteffectformat\#getRotatedChars--) |
| [setText(String value)](#setText-java.lang.String-) | Please see the getter of this property: [getText()](../../com.aspose.cells/texteffectformat\#getText--) |
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


Gets and sets the preset shape type.

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


Please see the getter of this property: [getFontBold()](../../com.aspose.cells/texteffectformat\#getFontBold--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Please see the getter of this property: [getFontItalic()](../../com.aspose.cells/texteffectformat\#getFontItalic--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Please see the getter of this property: [getFontName()](../../com.aspose.cells/texteffectformat\#getFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Please see the getter of this property: [getFontSize()](../../com.aspose.cells/texteffectformat\#getFontSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Please see the getter of this property: [getPresetShape()](../../com.aspose.cells/texteffectformat\#getPresetShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Please see the getter of this property: [getRotatedChars()](../../com.aspose.cells/texteffectformat\#getRotatedChars--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Please see the getter of this property: [getText()](../../com.aspose.cells/texteffectformat\#getText--)

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
| effect | int | The preset text effect. |

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

