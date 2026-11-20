---
title: "TextOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Textoptionen dar."
type: docs
url: /de/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Stellt die Textoptionen dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Überprüft, ob zwei Schriftarten gleich sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Liest die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [getCapsType()](#getCapsType--) | Liefert den Großschrifttyp für Texte der Form. |
| [getCharset()](#getCharset--) | Stellt den Zeichensatz dar. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Liefert das [Color](../../com.aspose.cells/color) der Schrift. |
| [getDoubleSize()](#getDoubleSize--) | Liefert die doppelte Größe der Schrift. |
| [getFarEastName()](#getFarEastName--) | Liefert den FarEast-Namen. |
| [getFill()](#getFill--) | Stellt das Füllformat des Textes dar. |
| [getKerning()](#getKerning--) | Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Zeichenpaarung (Kerning) erfolgt. |
| [getLanguageCode()](#getLanguageCode--) | Liefert die Sprache der Benutzeroberfläche. |
| [getLatinName()](#getLatinName--) | Liefert den lateinischen Namen. |
| [getName()](#getName--) | Ermittelt den Namen der Form. |
| [getOutline()](#getOutline--) | Stellt das Konturformat des Textes dar. |
| [getSchemeType()](#getSchemeType--) | Liefert den Schemata-Typ der Schrift. |
| [getScriptOffset()](#getScriptOffset--) | Liefert den Skriptversatz, in Prozent. |
| [getShadow()](#getShadow--) | Stellt ein [ShadowEffect](../../com.aspose.cells/shadoweffect)-Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt. |
| [getSize()](#getSize--) | Liefert die Größe der Schrift. |
| [getSpacing()](#getSpacing--) | Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an. |
| [getStrikeType()](#getStrikeType--) | Liefert den Durchstreichungstyp des Textes. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getUnderline()](#getUnderline--) | Ruft den Unterstreichungstyp der Schrift ab. |
| [getUnderlineColor()](#getUnderlineColor--) | Ruft die Farbe der Unterstreichung ab. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Ruft einen Wert ab, der angibt, ob die Schrift fett ist. |
| [isItalic()](#isItalic--) | Ruft einen Wert ab, der angibt, ob die Schrift kursiv ist. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist. |
| [isStrikeout()](#isStrikeout--) | Ruft einen Wert ab, der angibt, ob die Schrift einfach durchgestrichen ist. |
| [isSubscript()](#isSubscript--) | Ruft einen Wert ab, der angibt, ob die Schrift tiefgestellt ist. |
| [isSuperscript()](#isSuperscript--) | Ruft einen Wert ab, der angibt, ob die Schrift hochgestellt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [setBold(boolean value)](#setBold-boolean-) | Setzt einen Wert, der angibt, ob die Schrift fett ist. |
| [setCapsType(int value)](#setCapsType-int-) | Setzt den Großschreibungstyp für Texte der Form. |
| [setCharset(int value)](#setCharset-int-) | Stellt den Zeichensatz dar. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Setzt die [Farbe](../../com.aspose.cells/color) der Schrift. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Setzt die doppelte Größe der Schrift. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Setzt den FarEast-Namen. |
| [setItalic(boolean value)](#setItalic-boolean-) | Setzt einen Wert, der angibt, ob die Schrift kursiv ist. |
| [setKerning(double value)](#setKerning-double-) | Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Zeichenpaarung (Kerning) erfolgt. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Setzt die Sprache der Benutzeroberfläche. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Setzt den lateinischen Namen. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Form fest. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Setzt Name und Schema der Schrift. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist. |
| [setSchemeType(int value)](#setSchemeType-int-) | Setzt den Schematyp der Schrift. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Setzt den Skriptversatz in Prozent. |
| [setSize(int value)](#setSize-int-) | Setzt die Größe der Schrift. |
| [setSpacing(double value)](#setSpacing-double-) | Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an. |
| [setStrikeType(int value)](#setStrikeType-int-) | Liefert den Durchstreichungstyp des Textes. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Setzt einen Wert, der angibt, ob die Schrift einfach durchgestrichen ist. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Setzt einen Wert, der angibt, ob die Schrift tiefgestellt ist. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Setzt einen Wert, der angibt, ob die Schrift hochgestellt ist. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Legt die Designfarbe fest. |
| [setUnderline(int value)](#setUnderline-int-) | Setzt den Unterstreichungstyp der Schrift. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Setzt die Farbe der Unterstreichung. |
| [toString()](#toString--) | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Überprüft, ob zwei Schriftarten gleich sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Verglichenes Schriftobjekt. |

**Returns:**
boolescher Wert – True, wenn er dem verglichenen Schriftobjekt entspricht.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Liest die Farbe mit einem 32‑Bit‑ARGB‑Wert.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Liefert den Großschrifttyp für Texte der Form.

Siehe [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Stellt den Zeichensatz dar.

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


Liefert das [Color](../../com.aspose.cells/color) der Schrift.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Liefert die doppelte Größe der Schrift.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Liefert den FarEast-Namen.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Stellt das Füllformat des Textes dar.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Zeichenpaarung (Kerning) erfolgt.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Liefert die Sprache der Benutzeroberfläche.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Liefert den lateinischen Namen.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der Form.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Stellt das Konturformat des Textes dar.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Liefert den Schemata-Typ der Schrift.

Siehe [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Liefert den Skriptversatz, in Prozent.

**Remarks**

Nur für Formen und Diagramme.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Stellt ein [ShadowEffect](../../com.aspose.cells/shadoweffect)-Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Liefert die Größe der Schrift.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Liefert den Durchstreichungstyp des Textes.

Siehe [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Ermittelt die Designfarbe.

**Remarks**

Wenn die Schriftfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Ruft den Unterstreichungstyp der Schrift ab.

Siehe [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Ruft die Farbe der Unterstreichung ab.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Ruft einen Wert ab, der angibt, ob die Schrift fett ist.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Ruft einen Wert ab, der angibt, ob die Schrift kursiv ist.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist.

**Remarks**

Nur für die Schriften von Formen oder Diagrammen.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Ruft einen Wert ab, der angibt, ob die Schrift einfach durchgestrichen ist.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Ruft einen Wert ab, der angibt, ob die Schrift tiefgestellt ist.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Ruft einen Wert ab, der angibt, ob die Schrift hochgestellt ist.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift fett ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Setzt den Großschreibungstyp für Texte der Form.

Siehe [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Stellt den Zeichensatz dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Setzt die [Farbe](../../com.aspose.cells/color) der Schrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Setzt die doppelte Größe der Schrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Setzt den FarEast-Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift kursiv ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Zeichenpaarung (Kerning) erfolgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Setzt die Sprache der Benutzeroberfläche.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Setzt den lateinischen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen der Form fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Setzt Name und Schema der Schrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist.

**Remarks**

Nur für die Schriften von Formen oder Diagrammen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Setzt den Schematyp der Schrift.

Siehe [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Setzt den Skriptversatz in Prozent.

**Remarks**

Nur für Formen und Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Setzt die Größe der Schrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Liefert den Durchstreichungstyp des Textes.

Siehe [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift einfach durchgestrichen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift tiefgestellt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift hochgestellt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Legt die Designfarbe fest.

**Remarks**

Wenn die Schriftfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Setzt den Unterstreichungstyp der Schrift.

Siehe [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Setzt die Farbe der Unterstreichung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt.

**Returns:**
java.lang.String -
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

