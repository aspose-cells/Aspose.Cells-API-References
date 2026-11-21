---
title: "TextEffectFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Innehåller egenskaper och metoder som gäller för WordArt‑objekt."
type: docs
url: /sv/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Innehåller egenskaper och metoder som gäller för WordArt‑objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Indikerar om typsnittet är fetstil. |
| [getFontItalic()](#getFontItalic--) | Indikerar om typsnittet är kursivt. |
| [getFontName()](#getFontName--) | Namnet på teckensnittet som används i WordArt. |
| [getFontSize()](#getFontSize--) | Storleken (i punkter) på teckensnittet som används i WordArt. |
| [getPresetShape()](#getPresetShape--) | Hämtar den förinställda formtypen. |
| [getRotatedChars()](#getRotatedChars--) | Om true roteras tecken i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form. |
| [getText()](#getText--) | Texten i WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Indikerar om typsnittet är fetstil. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Indikerar om typsnittet är kursivt. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Namnet på teckensnittet som används i WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | Storleken (i punkter) på teckensnittet som används i WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Ställer in den förinställda formtypen. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Om true roteras tecken i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form. |
| [setText(String value)](#setText-java.lang.String-) | Texten i WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Ställer in den förinställda texteffekten. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Indikerar om typsnittet är fetstil.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Indikerar om typsnittet är kursivt.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


Namnet på teckensnittet som används i WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Storleken (i punkter) på teckensnittet som används i WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Hämtar den förinställda formtypen.

Se [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Om true roteras tecken i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Texten i WordArt.

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


Indikerar om typsnittet är fetstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Indikerar om typsnittet är kursivt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Namnet på teckensnittet som används i WordArt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Storleken (i punkter) på teckensnittet som används i WordArt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Ställer in den förinställda formtypen.

Se [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Om true roteras tecken i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Texten i WordArt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Ställer in den förinställda texteffekten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Den förinställda texteffekten. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

