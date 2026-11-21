---
title: "TextOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Metin seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Metin seçeneklerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | İki yazı tipinin eşit olup olmadığını denetler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | 32 bit ARGB değeriyle rengi alır. |
| [getCapsType()](#getCapsType--) | Şeklin metinleri için büyük harf tipini alır. |
| [getCharset()](#getCharset--) | Karakter kümesini temsil eder. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Yazı tipinin [Color](../../com.aspose.cells/color) değerini alır. |
| [getDoubleSize()](#getDoubleSize--) | Yazı tipinin çift boyutunu alır. |
| [getFarEastName()](#getFarEastName--) | FarEast adını alır. |
| [getFill()](#getFill--) | Metnin doldurma biçimini temsil eder. |
| [getKerning()](#getKerning--) | Bu metin çalışması için karakter aralığının (kerning) gerçekleşeceği minimum yazı tipi boyutunu belirtir. |
| [getLanguageCode()](#getLanguageCode--) | Kullanıcı arayüzü dilini alır. |
| [getLatinName()](#getLatinName--) | Latin adını alır. |
| [getName()](#getName--) | Şeklin adını alır. |
| [getOutline()](#getOutline--) | Metnin anahat biçimini temsil eder. |
| [getSchemeType()](#getSchemeType--) | Yazı tipinin şema türünü alır. |
| [getScriptOffset()](#getScriptOffset--) | Betik ofsetini yüzde biriminde alır |
| [getShadow()](#getShadow--) | Grafik öğesi veya şekil için gölge etkisini belirten bir [ShadowEffect](../../com.aspose.cells/shadoweffect) nesnesini temsil eder. |
| [getSize()](#getSize--) | Yazı tipinin boyutunu alır. |
| [getSpacing()](#getSpacing--) | Bir metin akışı içindeki karakterler arasındaki boşluğu belirtir. |
| [getStrikeType()](#getStrikeType--) | Metnin üstü çizili tipini alır. |
| [getThemeColor()](#getThemeColor--) | Tema rengini alır. |
| [getUnderline()](#getUnderline--) | Yazı tipinin alt çizgi tipini alır. |
| [getUnderlineColor()](#getUnderlineColor--) | Alt çizginin rengini alır. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Yazı tipinin kalın olup olmadığını gösteren bir değeri alır. |
| [isItalic()](#isItalic--) | Yazı tipinin italik olup olmadığını gösteren bir değeri alır. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Metin akışına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir. |
| [isStrikeout()](#isStrikeout--) | Yazı tipinin tek çizgi üzeri (strikeout) olup olmadığını gösteren bir değeri alır. |
| [isSubscript()](#isSubscript--) | Yazı tipinin alt simge (subscript) olup olmadığını gösteren bir değeri alır. |
| [isSuperscript()](#isSuperscript--) | Yazı tipinin üst simge (superscript) olup olmadığını gösteren bir değeri alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | 32 bit ARGB değeriyle rengi ayarlar. |
| [setBold(boolean value)](#setBold-boolean-) | Yazı tipinin kalın olup olmadığını gösteren bir değeri ayarlar. |
| [setCapsType(int value)](#setCapsType-int-) | Şeklin metinleri için büyük harf tipini ayarlar. |
| [setCharset(int value)](#setCharset-int-) | Karakter kümesini temsil eder. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Yazı tipinin [Color](../../com.aspose.cells/color) değerini ayarlar. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Yazı tipinin iki katı boyutunu ayarlar. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | FarEast adını ayarlar. |
| [setItalic(boolean value)](#setItalic-boolean-) | Yazı tipinin italik olup olmadığını gösteren bir değeri ayarlar. |
| [setKerning(double value)](#setKerning-double-) | Bu metin çalışması için karakter aralığının (kerning) gerçekleşeceği minimum yazı tipi boyutunu belirtir. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Kullanıcı arayüzü dilini ayarlar. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Latin adını ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Şeklin adını ayarlar. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Yazı tipinin adını ve şemasını ayarlar. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Metin akışına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir. |
| [setSchemeType(int value)](#setSchemeType-int-) | Yazı tipinin şema türünü ayarlar. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Betik ofsetini yüzde biriminde ayarlar. |
| [setSize(int value)](#setSize-int-) | Yazı tipinin boyutunu ayarlar. |
| [setSpacing(double value)](#setSpacing-double-) | Bir metin akışı içindeki karakterler arasındaki boşluğu belirtir. |
| [setStrikeType(int value)](#setStrikeType-int-) | Metnin üstü çizili tipini alır. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Yazı tipinin tek çizgi üstü olup olmadığını gösteren bir değer ayarlar. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Yazı tipinin alt simge olup olmadığını gösteren bir değer ayarlar. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Yazı tipinin üst simge olup olmadığını gösteren bir değer ayarlar. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Tema rengini ayarlar. |
| [setUnderline(int value)](#setUnderline-int-) | Yazı tipinin alt çizgi türünü ayarlar. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Alt çizginin rengini ayarlar. |
| [toString()](#toString--) | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


İki yazı tipinin eşit olup olmadığını denetler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Karşılaştırılan yazı tipi nesnesi. |

**Returns:**
boolean - Karşılaştırılan yazı tipi nesnesine eşitse True.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


32 bit ARGB değeriyle rengi alır.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Şeklin metinleri için büyük harf tipini alır.

Bkz [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Karakter kümesini temsil eder.

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


Yazı tipinin [Color](../../com.aspose.cells/color) değerini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Yazı tipinin çift boyutunu alır.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


FarEast adını alır.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Metnin doldurma biçimini temsil eder.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Bu metin çalışması için karakter aralığının (kerning) gerçekleşeceği minimum yazı tipi boyutunu belirtir.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Kullanıcı arayüzü dilini alır.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Latin adını alır.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Şeklin adını alır.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Metnin anahat biçimini temsil eder.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Yazı tipinin şema türünü alır.

Bkz [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Betik ofsetini yüzde biriminde alır

**Remarks**

Yalnızca şekiller ve grafikler için.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Grafik öğesi veya şekil için gölge etkisini belirten bir [ShadowEffect](../../com.aspose.cells/shadoweffect) nesnesini temsil eder.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Yazı tipinin boyutunu alır.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Bir metin akışı içindeki karakterler arasındaki boşluğu belirtir.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Metnin üstü çizili tipini alır.

Bkz [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Tema rengini alır.

**Remarks**

Yazı tipi rengi bir tema rengi değilse, NULL döndürülecektir.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Yazı tipinin alt çizgi tipini alır.

Bkz [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Alt çizginin rengini alır.

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


Yazı tipinin kalın olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Yazı tipinin italik olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Metin akışına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir.

**Remarks**

Yalnızca Şekiller veya Grafikler için yazı tipleri.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Yazı tipinin tek çizgi üzeri (strikeout) olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Yazı tipinin alt simge (subscript) olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Yazı tipinin üst simge (superscript) olup olmadığını gösteren bir değeri alır.

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


32 bit ARGB değeriyle rengi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Yazı tipinin kalın olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Şeklin metinleri için büyük harf tipini ayarlar.

Bkz [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Karakter kümesini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Yazı tipinin [Color](../../com.aspose.cells/color) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Yazı tipinin iki katı boyutunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


FarEast adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Yazı tipinin italik olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Bu metin çalışması için karakter aralığının (kerning) gerçekleşeceği minimum yazı tipi boyutunu belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Kullanıcı arayüzü dilini ayarlar.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Latin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Şeklin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Yazı tipinin adını ve şemasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Metin akışına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir.

**Remarks**

Yalnızca Şekiller veya Grafikler için yazı tipleri.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Yazı tipinin şema türünü ayarlar.

Bkz [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Betik ofsetini yüzde biriminde ayarlar.

**Remarks**

Yalnızca şekiller ve grafikler için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Yazı tipinin boyutunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Bir metin akışı içindeki karakterler arasındaki boşluğu belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Metnin üstü çizili tipini alır.

Bkz [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Yazı tipinin tek çizgi üstü olup olmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Yazı tipinin alt simge olup olmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Yazı tipinin üst simge olup olmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Tema rengini ayarlar.

**Remarks**

Yazı tipi rengi bir tema rengi değilse, NULL döndürülecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Yazı tipinin alt çizgi türünü ayarlar.

Bkz [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Alt çizginin rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Geçerli Cell nesnesini temsil eden bir dize döndürür.

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

