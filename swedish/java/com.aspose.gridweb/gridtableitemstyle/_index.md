---
title: "GridTableItemStyle"
second_title: "Aspose.Cells för Java API-referens"
description: "Härstammar från System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /sv/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Arv från System.Web.UI.WebControls.TableItemStyle. Inkapslar stilarna för en WebCell.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Standardkonstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Kopierar från ett annat stilobjekt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Hämtar BackColor i stilen |
| [getBackImageAttributes()](#getBackImageAttributes--) | Egenskaper för bakgrundsbild. |
| [getBackImageUrl()](#getBackImageUrl--) | URL för bakgrundsbild. |
| [getBorderColor()](#getBorderColor--) | Hämtar BorderColor i stilen |
| [getBorderStyle()](#getBorderStyle--) | Hämtar BorderStyle i stilen |
| [getBorderWidth()](#getBorderWidth--) | Hämtar BorderWidth i stilen |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Anger stilen för cellens nedre kant. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Hämtar CssClass i stilen |
| [getCustom()](#getCustom--) | Hämtar det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [getFont()](#getFont--) | Hämtar teckensnittet i stilen |
| [getForeColor()](#getForeColor--) | Hämtar förgrundsfärgen i stilen |
| [getHeight()](#getHeight--) | Hämtar höjden i stilen |
| [getHorizontalAlign()](#getHorizontalAlign--) | Hämtar horisontell justering i stilen |
| [getIndentLevel()](#getIndentLevel--) | Hämtar indenteringsnivå. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Anger stilen för cellens vänstra kant. |
| [getNumberType()](#getNumberType--) | Hämtar visningsformatet för tal och datum. |
| [getQuotePrefix()](#getQuotePrefix--) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Anger stilen för cellens högra kant. |
| [getRotationAngle()](#getRotationAngle--) | Hämtar rotationsattributet. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Anger stilen för cellens övre kant. |
| [getVerticalAlign()](#getVerticalAlign--) | Hämtar VerticalAlign i stilen |
| [getWidth()](#getWidth--) | Hämtar bredden i stilen |
| [getWrap()](#getWrap--) | Hämtar Wrap i stilen |
| [hashCode()](#hashCode--) | Fungerar som en hashfunktion för en viss typ, lämplig för användning i hash‑algoritmer och datastrukturer som en hashtabell. |
| [isLocked()](#isLocked--) | Hämtar ett värde som indikerar om en cell kan modifieras eller inte när dess kalkylblad är skyddat. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Slår samman med ett annat stilobjekt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Ställer in bakgrundsfärgen i stilen |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Egenskaper för bakgrundsbild. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL för bakgrundsbild. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Ställer in kantfärgen i stilen |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Ställer in kantstilen i stilen |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Ställer in kantbredden i stilen |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Anger stilen för cellens nedre kant. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Ställer in CssClass i stilen |
| [setCustom(String value)](#setCustom-java.lang.String-) | Ställer in det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Ställer in förgrundsfärgen i stilen |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Ställer in höjden i stilen |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Ställer in horisontell justering i stilen |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Ställer in indenteringsnivå. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Anger stilen för cellens vänstra kant. |
| [setLocked(boolean value)](#setLocked-boolean-) | Ställer in ett värde som anger om en cell kan ändras eller inte när dess kalkylblad är skyddat. |
| [setNumberType(int value)](#setNumberType-int-) | Ställer in visningsformatet för tal och datum. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Anger stilen för cellens högra kant. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Ställer in rotationsattributet. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Anger stilen för cellens övre kant. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Ställer in VerticalAlign i stilen |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Ställer in bredden i stilen |
| [setWrap(boolean value)](#setWrap-boolean-) | Ställer in Wrap i stilen |
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


Kopierar från ett annat stilobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | ett annat stilobjekt |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Hämtar BackColor i stilen

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Egenskaper för bakgrundsbild.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL för bakgrundsbild.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Hämtar BorderColor i stilen

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Hämtar BorderStyle i stilen

Se [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Hämtar BorderWidth i stilen

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Anger stilen för cellens nedre kant.

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


Hämtar CssClass i stilen

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Hämtar det anpassade formatet, null eller tom sträng betyder inget anpassat format.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Hämtar teckensnittet i stilen

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Hämtar förgrundsfärgen i stilen

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Hämtar höjden i stilen

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Hämtar horisontell justering i stilen

Se [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Hämtar indenteringsnivå.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Anger stilen för cellens vänstra kant.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Hämtar visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner.

**Remarks**

Till exempel, formateringsmönstren som representeras av siffror för regionen en\_US:

| Värde | Typ | Formateringssträng |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm FM/EM` |
| 19 | Time | `h:mm:ss FM/EM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Röd](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Röd](../#,##0.00)` |
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


Anger om cellens värde börjar med ett enkelt citattecken.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Anger stilen för cellens högra kant.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Hämtar rotationsattributet.

**Remarks**

0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.

Du kan ange 255 eller ett värde mellan -90 och 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Anger stilen för cellens övre kant.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Hämtar VerticalAlign i stilen

Se [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Hämtar bredden i stilen

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Hämtar Wrap i stilen

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Fungerar som en hashfunktion för en viss typ, lämplig för användning i hash‑algoritmer och datastrukturer som en hashtabell.

**Returns:**
int - En hashkod för den aktuella Style.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Hämtar ett värde som anger om en cell kan ändras eller inte när dess kalkylblad är skyddat. När kalkylbladet är skyddat och IsLocked är true, kan cellen inte redigeras. När kalkylbladet är skyddat och IsLocked är false, kan cellen redigeras.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Slår samman med ett annat stilobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | ett annat stilobjekt |

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


Ställer in bakgrundsfärgen i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Egenskaper för bakgrundsbild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL för bakgrundsbild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Ställer in kantfärgen i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Ställer in kantstilen i stilen

Se [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Ställer in kantbredden i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Anger stilen för cellens nedre kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Ställer in CssClass i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Ställer in det anpassade formatet, null eller tom sträng betyder inget anpassat format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Ställer in förgrundsfärgen i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Ställer in höjden i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Ställer in horisontell justering i stilen

Se [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Ställer in indenteringsnivå.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Anger stilen för cellens vänstra kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Ställer in ett värde som anger om en cell kan ändras eller inte när dess kalkylblad är skyddat. När kalkylbladet är skyddat och IsLocked är true, kan cellen inte redigeras. När kalkylbladet är skyddat och IsLocked är false, kan cellen redigeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Ställer in visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner.

**Remarks**

Till exempel, formateringsmönstren som representeras av siffror för regionen en\_US:

| Värde | Typ | Formateringssträng |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm FM/EM` |
| 19 | Time | `h:mm:ss FM/EM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Röd](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Röd](../#,##0.00)` |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Anger om cellens värde börjar med ett enkelt citattecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Anger stilen för cellens högra kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Ställer in rotationsattributet.

**Remarks**

0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.

Du kan ange 255 eller ett värde mellan -90 och 90.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Anger stilen för cellens övre kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Ställer in VerticalAlign i stilen

Se [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Ställer in bredden i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Ställer in Wrap i stilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

