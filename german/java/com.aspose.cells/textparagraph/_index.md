---
title: "TextParagraph"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellung des Textabsatzes dar."
type: docs
url: /de/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Stellt die Einstellung des Textabsatzes dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Liefert den horizontalen Ausrichtungstyp des Textes im Absatz. |
| [getBullet()](#getBullet--) | Liefert das Aufzählungszeichen. |
| [getChildren()](#getChildren--) | Liefert alle Textläufe in diesem Absatz. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Liefert die Standardgröße für ein Tabulatorzeichen in diesem Absatz. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird. |
| [getFont()](#getFont--) | Gibt die Schriftart dieses Objekts zurück. |
| [getFontAlignType()](#getFontAlignType--) | Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert werden. |
| [getLeftMargin()](#getLeftMargin--) | Gibt den linken Rand des Absatzes an. |
| [getLength()](#getLength--) | Ermittelt die Länge der Zeichen. |
| [getLineSpace()](#getLineSpace--) | Ermittelt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Ermittelt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [getRightMargin()](#getRightMargin--) | Gibt den rechten Rand des Absatzes an. |
| [getSpaceAfter()](#getSpaceAfter--) | Ermittelt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Ermittelt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [getSpaceBefore()](#getSpaceBefore--) | Ermittelt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Ermittelt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [getStartIndex()](#getStartIndex--) | Ermittelt den Startindex der Zeichen. |
| [getStops()](#getStops--) | Ermittelt die Tabulator-Stoppliste. |
| [getTextOptions()](#getTextOptions--) | Gibt die Textoptionen zurück. |
| [getType()](#getType--) | Ermittelt den Typ des Textknotens. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Legt den horizontalen Ausrichtungstyp des Textes im Absatz fest. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Legt die Standardgröße für ein Tabulatorzeichen in diesem Absatz fest. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert werden. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Gibt den linken Rand des Absatzes an. |
| [setLineSpace(double value)](#setLineSpace-double-) | Legt die Menge des vertikalen Leerraums fest, die innerhalb eines Absatzes verwendet wird. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Legt die Menge des vertikalen Leerraums fest, die innerhalb eines Absatzes verwendet wird. |
| [setRightMargin(double value)](#setRightMargin-double-) | Gibt den rechten Rand des Absatzes an. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Legt die Menge des vertikalen Leerraums fest, die nach einem Absatz vorhanden ist. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Legt die Menge des vertikalen Leerraums fest, die nach einem Absatz vorhanden ist. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Legt die Menge des vertikalen Leerraums fest, die vor einem Absatz vorhanden ist. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Legt die Menge des vertikalen Leerraums fest, die vor einem Absatz vorhanden ist. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Legt den vordefinierten WordArt-Stil fest. |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Liefert den horizontalen Ausrichtungstyp des Textes im Absatz.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Liefert das Aufzählungszeichen.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Ermittelt alle Textläufe in diesem Absatz. Wenn dieser Absatz leer ist, wird der Absatz selbst zurückgegeben.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Liefert die Standardgröße für ein Tabulatorzeichen in diesem Absatz.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Gibt die Schriftart dieses Objekts zurück.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert sind. Dies betrifft die vertikale Platzierung der Zeichen in Bezug auf die Grundlinien.

Siehe [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Gibt den linken Rand des Absatzes an.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Ermittelt die Länge der Zeichen.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Ermittelt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Ermittelt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Gibt den rechten Rand des Absatzes an.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Ermittelt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Ermittelt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Ermittelt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Ermittelt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Ermittelt den Startindex der Zeichen.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Ermittelt die Tabulator-Stoppliste.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Gibt die Textoptionen zurück.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ des Textknotens.

Siehe [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Legt den horizontalen Ausrichtungstyp des Textes im Absatz fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Legt die Standardgröße für ein Tabulatorzeichen in diesem Absatz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert sind. Dies betrifft die vertikale Platzierung der Zeichen in Bezug auf die Grundlinien.

Siehe [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Gibt den linken Rand des Absatzes an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Legt die Menge des vertikalen Leerraums fest, die innerhalb eines Absatzes verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Legt die Menge des vertikalen Leerraums fest, die innerhalb eines Absatzes verwendet wird.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Gibt den rechten Rand des Absatzes an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Legt die Menge des vertikalen Leerraums fest, die nach einem Absatz vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Legt die Menge des vertikalen Leerraums fest, die nach einem Absatz vorhanden ist.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Legt die Menge des vertikalen Leerraums fest, die vor einem Absatz vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Legt die Menge des vertikalen Leerraums fest, die vor einem Absatz vorhanden ist.

Siehe [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Legt den vordefinierten WordArt-Stil fest.

**Remarks**

Nur für den Text von Form/Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Der voreingestellte WordArt-Stil. |

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

