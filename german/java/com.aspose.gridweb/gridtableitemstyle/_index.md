---
title: "GridTableItemStyle"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Abgeleitet von System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /de/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Erbt von System.Web.UI.WebControls.TableItemStyle. Kapselt die Stile einer WebCell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Standardkonstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Kopiert von einem anderen Stilobjekt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Ruft die BackColor im Stil ab |
| [getBackImageAttributes()](#getBackImageAttributes--) | Attribute des Hintergrundbildes. |
| [getBackImageUrl()](#getBackImageUrl--) | URL des Hintergrundbildes. |
| [getBorderColor()](#getBorderColor--) | Ruft die BorderColor im Stil ab |
| [getBorderStyle()](#getBorderStyle--) | Ruft die BorderStyle im Stil ab |
| [getBorderWidth()](#getBorderWidth--) | Ruft die BorderWidth im Stil ab |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Gibt den Stil des unteren Rands der Zelle an. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Ruft die CssClass im Stil ab |
| [getCustom()](#getCustom--) | Liefert das benutzerdefinierte Format, null oder leere Zeichenkette bedeutet kein benutzerdefiniertes Format. |
| [getFont()](#getFont--) | Ruft die Font im Stil ab |
| [getForeColor()](#getForeColor--) | Ruft die ForeColor im Stil ab |
| [getHeight()](#getHeight--) | Ruft die Height im Stil ab |
| [getHorizontalAlign()](#getHorizontalAlign--) | Ruft die HorizontalAlign im Stil ab |
| [getIndentLevel()](#getIndentLevel--) | Liefert die Einzugsebene. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Gibt den Stil des linken Rands der Zelle an. |
| [getNumberType()](#getNumberType--) | Ruft das Anzeigeformat von Zahlen und Datumsangaben ab. |
| [getQuotePrefix()](#getQuotePrefix--) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Gibt den Stil des rechten Rands der Zelle an. |
| [getRotationAngle()](#getRotationAngle--) | Ruft das Rotationsattribut ab. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Gibt den Stil des oberen Zellrandes an. |
| [getVerticalAlign()](#getVerticalAlign--) | Ruft die VerticalAlign im Stil ab. |
| [getWidth()](#getWidth--) | Ruft die Width im Stil ab |
| [getWrap()](#getWrap--) | Ruft die Wrap im Stil ab. |
| [hashCode()](#hashCode--) | Dient als Hashfunktion für einen bestimmten Typ, geeignet für den Einsatz in Hash-Algorithmen und Datenstrukturen wie einer Hashtabelle. |
| [isLocked()](#isLocked--) | Ruft einen Wert ab, der angibt, ob eine Zelle geändert werden kann, wenn ihr Arbeitsblatt geschützt ist. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Führt mit einem anderen Stilobjekt zusammen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Legt die BackColor im Stil fest |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Attribute des Hintergrundbildes. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL des Hintergrundbildes. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Legt die BorderColor im Stil fest |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Legt die BorderStyle im Stil fest |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Legt die BorderWidth im Stil fest |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Gibt den Stil des unteren Rands der Zelle an. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Legt die CssClass im Stil fest |
| [setCustom(String value)](#setCustom-java.lang.String-) | Legt das benutzerdefinierte Format fest, null oder ein leerer String bedeutet kein benutzerdefiniertes Format. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Legt die ForeColor im Stil fest |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Legt die Höhe im Stil fest |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Legt die horizontale Ausrichtung im Stil fest |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Legt die Einrückungsebene fest. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Gibt den Stil des linken Rands der Zelle an. |
| [setLocked(boolean value)](#setLocked-boolean-) | Legt einen Wert fest, der angibt, ob eine Zelle geändert werden kann, wenn ihr Arbeitsblatt geschützt ist. |
| [setNumberType(int value)](#setNumberType-int-) | Legt das Anzeigeformat von Zahlen und Datumsangaben fest. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Gibt den Stil des rechten Rands der Zelle an. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Legt das Rotationsattribut fest. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Gibt den Stil des oberen Zellrandes an. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Legt die VerticalAlign im Stil fest. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Legt die Breite im Stil fest |
| [setWrap(boolean value)](#setWrap-boolean-) | Legt die Wrap im Stil fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Standardkonstruktor.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Kopiert von einem anderen Stilobjekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | ein weiteres Stilobjekt |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Ruft die BackColor im Stil ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Attribute des Hintergrundbildes.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL des Hintergrundbildes.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Ruft die BorderColor im Stil ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ruft die BorderStyle im Stil ab

Siehe [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Ruft die BorderWidth im Stil ab

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Gibt den Stil des unteren Rands der Zelle an.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Ruft die CssClass im Stil ab

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Liefert das benutzerdefinierte Format, null oder leere Zeichenkette bedeutet kein benutzerdefiniertes Format.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Ruft die Font im Stil ab

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Ruft die ForeColor im Stil ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Ruft die Height im Stil ab

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Ruft die HorizontalAlign im Stil ab

Siehe [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Liefert die Einzugsebene.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Gibt den Stil des linken Rands der Zelle an.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Gibt das Anzeigeformat von Zahlen und Datumsangaben zurück. Die Formatierungsmuster unterscheiden sich je nach Region.

**Remarks**

Beispielweise werden die Formatierungsmuster für die Region en\\_US durch Zahlen dargestellt:

| Value | Typ | Formatzeichenfolge |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rot](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rot](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rot](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Gibt den Stil des rechten Rands der Zelle an.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Ruft das Rotationsattribut ab.

**Remarks**

0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.

Sie können 255 oder einen Wert im Bereich von -90 bis 90 setzen.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Gibt den Stil des oberen Zellrandes an.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Ruft die VerticalAlign im Stil ab.

Siehe [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ruft die Width im Stil ab

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Ruft die Wrap im Stil ab.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hashfunktion für einen bestimmten Typ, geeignet für den Einsatz in Hash-Algorithmen und Datenstrukturen wie einer Hashtabelle.

**Returns:**
int – Ein Hashcode für den aktuellen Stil.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Ruft einen Wert ab, der angibt, ob eine Zelle geändert werden kann, wenn ihr Arbeitsblatt geschützt ist. Wenn das Arbeitsblatt geschützt ist und IsLocked true ist, kann die Zelle nicht bearbeitet werden. Wenn das Arbeitsblatt geschützt ist und IsLocked false ist, kann die Zelle bearbeitet werden.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Führt mit einem anderen Stilobjekt zusammen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | ein weiteres Stilobjekt |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Legt die BackColor im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Attribute des Hintergrundbildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL des Hintergrundbildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Legt die BorderColor im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Legt die BorderStyle im Stil fest

Siehe [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Legt die BorderWidth im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Gibt den Stil des unteren Rands der Zelle an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Legt die CssClass im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Legt das benutzerdefinierte Format fest, null oder ein leerer String bedeutet kein benutzerdefiniertes Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Legt die ForeColor im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Legt die Höhe im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Legt die horizontale Ausrichtung im Stil fest

Siehe [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Legt die Einrückungsebene fest.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Gibt den Stil des linken Rands der Zelle an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Legt einen Wert fest, der angibt, ob eine Zelle geändert werden kann, wenn ihr Arbeitsblatt geschützt ist. Wenn das Arbeitsblatt geschützt ist und IsLocked true ist, kann die Zelle nicht bearbeitet werden. Wenn das Arbeitsblatt geschützt ist und IsLocked false ist, kann die Zelle bearbeitet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Legt das Anzeigeformat von Zahlen und Datumsangaben fest. Die Formatierungsmuster unterscheiden sich je nach Region.

**Remarks**

Beispielweise werden die Formatierungsmuster für die Region en\\_US durch Zahlen dargestellt:

| Value | Typ | Formatzeichenfolge |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rot](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rot](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rot](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Gibt den Stil des rechten Rands der Zelle an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Legt das Rotationsattribut fest.

**Remarks**

0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.

Sie können 255 oder einen Wert im Bereich von -90 bis 90 setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Gibt den Stil des oberen Zellrandes an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Legt die VerticalAlign im Stil fest.

Siehe [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Legt die Breite im Stil fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Legt die Wrap im Stil fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

