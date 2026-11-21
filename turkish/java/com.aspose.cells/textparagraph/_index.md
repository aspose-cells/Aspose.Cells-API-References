---
title: "TextParagraph"
second_title: "Aspose.Cells for Java API Referansı"
description: "Metin paragraf ayarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Metin paragraf ayarını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Paragrafın metin yatay hizalama türünü alır. |
| [getBullet()](#getBullet--) | Madde işaretini alır. |
| [getChildren()](#getChildren--) | Bu paragraftaki tüm metin akışlarını alır. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Bu paragrafta bir sekme karakteri için varsayılan boyutu alır. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir. |
| [getFont()](#getFont--) | Bu nesnenin yazı tipini döndürür. |
| [getFontAlignType()](#getFontAlignType--) | Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. |
| [getLeftMargin()](#getLeftMargin--) | Paragrafın sol kenar boşluğunu belirtir. |
| [getLength()](#getLength--) | Karakterlerin uzunluğunu alır. |
| [getLineSpace()](#getLineSpace--) | Paragraf içinde kullanılacak dikey boşluk miktarını alır. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Paragraf içinde kullanılacak dikey boşluk miktarını alır. |
| [getRightMargin()](#getRightMargin--) | Paragrafın sağ kenar boşluğunu belirtir. |
| [getSpaceAfter()](#getSpaceAfter--) | Paragraftan sonra bulunacak dikey boşluk miktarını alır. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Paragraftan sonra bulunacak dikey boşluk miktarını alır. |
| [getSpaceBefore()](#getSpaceBefore--) | Paragraftan önce bulunacak dikey boşluk miktarını alır. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Paragraftan önce bulunacak dikey boşluk miktarını alır. |
| [getStartIndex()](#getStartIndex--) | Karakterlerin başlangıç indeksini alır. |
| [getStops()](#getStops--) | Sekme durakları listesini alır. |
| [getTextOptions()](#getTextOptions--) | Metin seçeneklerini döndürür. |
| [getType()](#getType--) | Metin düğümünün tipini alır. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Bir Doğu Asya kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Bir Latin kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Paragrafın metin yatay hizalama türünü ayarlar. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Bu paragrafta bir sekme karakteri için varsayılan boyutu ayarlar. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Bir Doğu Asya kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Bir Latin kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Paragrafın sol kenar boşluğunu belirtir. |
| [setLineSpace(double value)](#setLineSpace-double-) | Paragraf içinde kullanılacak dikey boşluk miktarını ayarlar. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Paragraf içinde kullanılacak dikey boşluk miktarını ayarlar. |
| [setRightMargin(double value)](#setRightMargin-double-) | Paragrafın sağ kenar boşluğunu belirtir. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Paragraftan sonra bulunacak dikey boşluk miktarını ayarlar. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Paragraftan sonra bulunacak dikey boşluk miktarını ayarlar. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Paragraftan önce bulunacak dikey boşluk miktarını ayarlar. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Paragraftan önce bulunacak dikey boşluk miktarını ayarlar. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Önceden ayarlanmış WordArt stilini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Paragrafın metin yatay hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Madde işaretini alır.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Bu paragraftaki tüm metin akışlarını alır. Eğer bu paragraf boşsa, paragrafı kendisini döndür.

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


Bu paragrafta bir sekme karakteri için varsayılan boyutu alır.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Bu nesnenin yazı tipini döndürür.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini ele alır.

Bkz [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Paragrafın sol kenar boşluğunu belirtir.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Karakterlerin uzunluğunu alır.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Paragraf içinde kullanılacak dikey boşluk miktarını alır.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Paragraf içinde kullanılacak dikey boşluk miktarını alır.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Paragrafın sağ kenar boşluğunu belirtir.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Paragraftan sonra bulunacak dikey boşluk miktarını alır.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Paragraftan sonra bulunacak dikey boşluk miktarını alır.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Paragraftan önce bulunacak dikey boşluk miktarını alır.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Paragraftan önce bulunacak dikey boşluk miktarını alır.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Karakterlerin başlangıç indeksini alır.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Sekme durakları listesini alır.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Metin seçeneklerini döndürür.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Metin düğümünün tipini alır.

Bkz. [TextNodeType](../../com.aspose.cells/textnodetype).

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


Bir Doğu Asya kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Bir Latin kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir.

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


Paragrafın metin yatay hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Bu paragrafta bir sekme karakteri için varsayılan boyutu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Bir Doğu Asya kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini ele alır.

Bkz [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Bir Latin kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Paragrafın sol kenar boşluğunu belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Paragraf içinde kullanılacak dikey boşluk miktarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Paragraf içinde kullanılacak dikey boşluk miktarını ayarlar.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Paragrafın sağ kenar boşluğunu belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Paragraftan sonra bulunacak dikey boşluk miktarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Paragraftan sonra bulunacak dikey boşluk miktarını ayarlar.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Paragraftan önce bulunacak dikey boşluk miktarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Paragraftan önce bulunacak dikey boşluk miktarını ayarlar.

Bkz [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Önceden ayarlanmış WordArt stilini ayarlar.

**Remarks**

Yalnızca şekil/grafik metni için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Önceden ayarlanmış WordArt stili. |

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

