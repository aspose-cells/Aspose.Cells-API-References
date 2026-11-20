---
title: "TextEffectFormat"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Enthält Eigenschaften und Methoden, die auf WordArt-Objekte zutreffen."
type: docs
url: /de/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Enthält Eigenschaften und Methoden, die auf WordArt-Objekte zutreffen.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Gibt an, ob die Schrift fett ist. |
| [getFontItalic()](#getFontItalic--) | Gibt an, ob die Schrift kursiv ist. |
| [getFontName()](#getFontName--) | Der Name der im WordArt verwendeten Schriftart. |
| [getFontSize()](#getFontSize--) | Die Größe (in Punkten) der im WordArt verwendeten Schriftart. |
| [getPresetShape()](#getPresetShape--) | Liefert den voreingestellten Formtyp. |
| [getRotatedChars()](#getRotatedChars--) | Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht. |
| [getText()](#getText--) | Der Text im WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Gibt an, ob die Schrift fett ist. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Gibt an, ob die Schrift kursiv ist. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Der Name der im WordArt verwendeten Schriftart. |
| [setFontSize(int value)](#setFontSize-int-) | Die Größe (in Punkten) der im WordArt verwendeten Schriftart. |
| [setPresetShape(int value)](#setPresetShape-int-) | Legt den voreingestellten Formtyp fest. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht. |
| [setText(String value)](#setText-java.lang.String-) | Der Text im WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Legt den voreingestellten Texteffekt fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Gibt an, ob die Schrift fett ist.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Gibt an, ob die Schrift kursiv ist.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


Der Name der im WordArt verwendeten Schriftart.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Die Größe (in Punkten) der im WordArt verwendeten Schriftart.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Liefert den voreingestellten Formtyp.

Siehe [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Der Text im WordArt.

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


Gibt an, ob die Schrift fett ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Gibt an, ob die Schrift kursiv ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Der Name der im WordArt verwendeten Schriftart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Die Größe (in Punkten) der im WordArt verwendeten Schriftart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Legt den voreingestellten Formtyp fest.

Siehe [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Der Text im WordArt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Legt den voreingestellten Texteffekt fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Der voreingestellte Texteffekt. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

