---
title: "Font"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Schriftobjekt, das in einer Tabellenkalkulation verwendet wird."
type: docs
url: /de/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Kapselt das Schriftobjekt, das in einer Tabellenkalkulation verwendet wird.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Überprüft, ob zwei Schriftarten gleich sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Liest die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [getCapsType()](#getCapsType--) | Ermittelt den Text‑Großschreibungstyp. |
| [getCharset()](#getCharset--) | Stellt den Zeichensatz dar. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Liefert das [Color](../../com.aspose.cells/color) der Schrift. |
| [getDoubleSize()](#getDoubleSize--) | Liefert die doppelte Größe der Schrift. |
| [getName()](#getName--) | Ermittelt den Namen der [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | Liefert den Schemata-Typ der Schrift. |
| [getScriptOffset()](#getScriptOffset--) | Liefert den Skriptversatz, in Prozent. |
| [getSize()](#getSize--) | Liefert die Größe der Schrift. |
| [getStrikeType()](#getStrikeType--) | Liefert den Durchstreichungstyp des Textes. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getUnderline()](#getUnderline--) | Ruft den Unterstreichungstyp der Schrift ab. |
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
| [setCapsType(int value)](#setCapsType-int-) | Setzt den Text‑Großschreibungstyp. |
| [setCharset(int value)](#setCharset-int-) | Stellt den Zeichensatz dar. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Setzt die [Farbe](../../com.aspose.cells/color) der Schrift. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Setzt die doppelte Größe der Schrift. |
| [setItalic(boolean value)](#setItalic-boolean-) | Setzt einen Wert, der angibt, ob die Schrift kursiv ist. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen der [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Setzt Name und Schema der Schrift. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist. |
| [setSchemeType(int value)](#setSchemeType-int-) | Setzt den Schematyp der Schrift. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Setzt den Skriptversatz in Prozent. |
| [setSize(int value)](#setSize-int-) | Setzt die Größe der Schrift. |
| [setStrikeType(int value)](#setStrikeType-int-) | Liefert den Durchstreichungstyp des Textes. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Setzt einen Wert, der angibt, ob die Schrift einfach durchgestrichen ist. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Setzt einen Wert, der angibt, ob die Schrift tiefgestellt ist. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Setzt einen Wert, der angibt, ob die Schrift hochgestellt ist. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Legt die Designfarbe fest. |
| [setUnderline(int value)](#setUnderline-int-) | Setzt den Unterstreichungstyp der Schrift. |
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


Ermittelt den Text‑Großschreibungstyp.

Siehe [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Nur für die Schriftarten von Formen oder Diagrammen. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) . Diese Eigenschaft wird 12 Monate nach Januar 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

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
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der [Font](../../com.aspose.cells/font).

**Remarks**

Wenn diese Eigenschaft verwendet wird, um den Namen der Schriftart festzulegen, wird [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) auf [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE) aktualisiert.

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Liefert die Größe der Schrift.

**Returns:**
int
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

Nur für die Schriftarten von Formen oder Diagrammen. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) . Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

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


Setzt den Text‑Großschreibungstyp.

Siehe [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Nur für die Schriftarten von Formen oder Diagrammen. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) . Diese Eigenschaft wird 12 Monate nach Januar 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Setzt einen Wert, der angibt, ob die Schrift kursiv ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen der [Font](../../com.aspose.cells/font).

**Remarks**

Wenn diese Eigenschaft verwendet wird, um den Namen der Schriftart festzulegen, wird [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) auf [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE) aktualisiert.

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

Nur für die Schriftarten von Formen oder Diagrammen. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) . Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

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

