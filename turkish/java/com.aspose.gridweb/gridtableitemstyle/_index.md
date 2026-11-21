---
title: "GridTableItemStyle"
second_title: "Aspose.Cells for Java API Referansı"
description: "System.Web.UI.WebControls.TableItemStyle sınıfından miras alınmıştır."
type: docs
url: /tr/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

System.Web.UI.WebControls.TableItemStyle sınıfından kalıtılmıştır. Bir WebCell'in stillerini kapsar.

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
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Varsayılan yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Başka bir stil nesnesinden kopyalar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Stildeki BackColor değerini alır |
| [getBackImageAttributes()](#getBackImageAttributes--) | Arka plan görüntüsü özellikleri. |
| [getBackImageUrl()](#getBackImageUrl--) | Arka plan görüntüsü URL'si. |
| [getBorderColor()](#getBorderColor--) | Stildeki BorderColor değerini alır |
| [getBorderStyle()](#getBorderStyle--) | Stildeki BorderStyle değerini alır |
| [getBorderWidth()](#getBorderWidth--) | Stildeki BorderWidth değerini alır |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Hücrenin alt kenarının stilini belirtir. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Stildeki CssClass değerini alır |
| [getCustom()](#getCustom--) | Özel biçimi alır, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [getFont()](#getFont--) | Stildeki Font değerini alır |
| [getForeColor()](#getForeColor--) | Stildeki ForeColor değerini alır |
| [getHeight()](#getHeight--) | Stildeki Height değerini alır |
| [getHorizontalAlign()](#getHorizontalAlign--) | Stilde HorizontalAlign'i alır |
| [getIndentLevel()](#getIndentLevel--) | Girinti seviyesini alır. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Hücrenin sol kenarının stilini belirtir. |
| [getNumberType()](#getNumberType--) | Sayıların ve tarihlerin görüntüleme biçimini alır. |
| [getQuotePrefix()](#getQuotePrefix--) | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Hücrenin sağ kenarının stilini belirtir. |
| [getRotationAngle()](#getRotationAngle--) | Dönme özelliğini alır. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Hücrenin üst kenarının stilini belirtir. |
| [getVerticalAlign()](#getVerticalAlign--) | Stildeki Dikey Hizalamayı alır. |
| [getWidth()](#getWidth--) | Stilde Width'i alır |
| [getWrap()](#getWrap--) | Stildeki Kaydırmayı alır. |
| [hashCode()](#hashCode--) | Belirli bir tip için bir hash işlevi olarak hizmet verir, hash algoritmaları ve hash tablosu gibi veri yapılarında kullanılmaya uygundur. |
| [isLocked()](#isLocked--) | Çalışma sayfası korunduğunda bir hücrenin değiştirilebilir olup olmadığını gösteren değeri alır. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Başka bir stil nesnesiyle birleştirir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Stilde BackColor'i ayarlar |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Arka plan görüntüsü özellikleri. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | Arka plan görüntüsü URL'si. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Stilde BorderColor'i ayarlar |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Stilde BorderStyle'i ayarlar |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Stilde BorderWidth'i ayarlar |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Hücrenin alt kenarının stilini belirtir. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Stilde CssClass'i ayarlar |
| [setCustom(String value)](#setCustom-java.lang.String-) | Özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Stilde ForeColor'i ayarlar |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Stilde Height'i ayarlar |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Stilde HorizontalAlign'i ayarlar |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Girinti seviyesini ayarlar. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Hücrenin sol kenarının stilini belirtir. |
| [setLocked(boolean value)](#setLocked-boolean-) | Çalışma sayfası korunduğunda bir hücrenin değiştirilebilir olup olmadığını gösteren değeri ayarlar. |
| [setNumberType(int value)](#setNumberType-int-) | Sayıların ve tarihlerin görüntüleme biçimini ayarlar. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Hücrenin sağ kenarının stilini belirtir. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Dönme özelliğini ayarlar. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Hücrenin üst kenarının stilini belirtir. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Stildeki Dikey Hizalamayı ayarlar. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Stilde Width'i ayarlar |
| [setWrap(boolean value)](#setWrap-boolean-) | Stildeki Kaydırmayı ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Varsayılan yapıcı.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Başka bir stil nesnesinden kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | başka bir stil nesnesi |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Stildeki BackColor değerini alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Arka plan görüntüsü özellikleri.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


Arka plan görüntüsü URL'si.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Stildeki BorderColor değerini alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Stildeki BorderStyle değerini alır

Bakınız [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Stildeki BorderWidth değerini alır

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Hücrenin alt kenarının stilini belirtir.

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


Stildeki CssClass değerini alır

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Özel biçimi alır, null veya boş dize özel biçim olmadığı anlamına gelir.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Stildeki Font değerini alır

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Stildeki ForeColor değerini alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Stildeki Height değerini alır

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Stilde HorizontalAlign'i alır

Bakınız [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Girinti seviyesini alır.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Hücrenin sol kenarının stilini belirtir.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Sayıların ve tarihlerin görüntüleme biçimini alır. Biçimlendirme desenleri farklı bölgeler için farklıdır.

**Remarks**

Örneğin, en\\_US bölgesi için sayılarla temsil edilen biçimlendirme desenleri:

| Değer | Tür | Biçim Dizesi |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Kırmızı](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Kırmızı](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ÖÖ/ÖS` |
| 19 | Time | `h:mm:ss ÖÖ/ÖS` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Kırmızı](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Kırmızı](../#,##0.00)` |
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


Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Hücrenin sağ kenarının stilini belirtir.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Dönme özelliğini alır.

**Remarks**

0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.

255 veya -90 ile 90 arasında bir değer ayarlayabilirsiniz.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Hücrenin üst kenarının stilini belirtir.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Stildeki Dikey Hizalamayı alır.

Bakınız [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Stilde Width'i alır

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Stildeki Kaydırmayı alır.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Belirli bir tip için bir hash işlevi olarak hizmet verir, hash algoritmaları ve hash tablosu gibi veri yapılarında kullanılmaya uygundur.

**Returns:**
int - Geçerli Stil için bir karma kodu.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Bir değer alır, hücrenin çalışma sayfası korunduğunda değiştirilebilir olup olmadığını gösterir. Çalışma sayfası korunduğunda ve IsLocked true olduğunda, hücre düzenlenemez. Çalışma sayfası korunduğunda ve IsLocked false olduğunda, hücre düzenlenebilir.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Başka bir stil nesnesiyle birleştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | başka bir stil nesnesi |

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


Stilde BackColor'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Arka plan görüntüsü özellikleri.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


Arka plan görüntüsü URL'si.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Stilde BorderColor'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Stilde BorderStyle'i ayarlar

Bakınız [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Stilde BorderWidth'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Hücrenin alt kenarının stilini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Stilde CssClass'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Stilde ForeColor'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Stilde Height'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Stilde HorizontalAlign'i ayarlar

Bakınız [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Girinti seviyesini ayarlar.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Hücrenin sol kenarının stilini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Bir değer ayarlar, hücrenin çalışma sayfası korunduğunda değiştirilebilir olup olmadığını gösterir. Çalışma sayfası korunduğunda ve IsLocked true olduğunda, hücre düzenlenemez. Çalışma sayfası korunduğunda ve IsLocked false olduğunda, hücre düzenlenebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Sayıların ve tarihlerin görüntüleme biçimini ayarlar. Biçimlendirme desenleri farklı bölgeler için farklıdır.

**Remarks**

Örneğin, en\\_US bölgesi için sayılarla temsil edilen biçimlendirme desenleri:

| Değer | Tür | Biçim Dizesi |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Kırmızı](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Kırmızı](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ÖÖ/ÖS` |
| 19 | Time | `h:mm:ss ÖÖ/ÖS` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Kırmızı](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Kırmızı](../#,##0.00)` |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Hücrenin sağ kenarının stilini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Dönme özelliğini ayarlar.

**Remarks**

0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.

255 veya -90 ile 90 arasında bir değer ayarlayabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Hücrenin üst kenarının stilini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Stildeki Dikey Hizalamayı ayarlar.

Bakınız [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Stilde Width'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Stildeki Kaydırmayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

