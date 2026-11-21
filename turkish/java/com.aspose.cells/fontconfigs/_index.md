---
title: "FontConfigs"
second_title: "Aspose.Cells for Java API Referansı"
description: "Yazı tipi ayarlarını belirtir"
type: docs
url: /tr/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Yazı tipi ayarlarını belirtir
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Varsayılan yazı tipi adını alır. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Yazı tipi dosyası verisinin veri bilgilerini al. |
| [getFontSources()](#getFontSources--) | Kaynakların listesini içeren dizinin bir kopyasını alır. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi yedek adlarını içeren bir dizi döndürür. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Yazı tipinin mevcut olup olmadığını göster. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Varsayılan yazı tipi adını ayarlar. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Yazı tiplerinin yalnızca kaynaklarını ayarlar. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Yazı tipi klasörünü ayarlar |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Yazı tipi klasörünü ayarlar |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Yazı tipi kaynaklarını ayarlar. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Verilen orijinal yazı tipi adı için yazı tipi ikame adları. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontConfigs() {#FontConfigs--}
```
public FontConfigs()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


Varsayılan yazı tipi adını alır.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Yazı tipi dosyası verisinin veri bilgilerini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | java.lang.String | yazı tipi adı |
| isBold | boolean | yazı tipi stili kalın mı değil mi |
| isItalic | boolean | yazı tipi stili italik mi değil mi |
| isExactStyle | boolean | verilen kalın/italik stilinin tam olarak eşleşip eşleşmeyeceği |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Kaynakların listesini içeren dizinin bir kopyasını alır.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi yedek adlarını içeren bir dizi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


Yazı tipinin mevcut olup olmadığını göster.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | java.lang.String | yazı tipi adı |

**Returns:**
boolean - yazı tipi mevcutsa true, aksi takdirde false.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```


Varsayılan yazı tipi adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


Yazı tiplerinin yalnızca kaynaklarını ayarlar. Kaynaklardaki yalnızca yazı tipleri kullanılacaktır.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") bu ayar yapıldıysa yok sayılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | TrueType yazı tiplerini içeren kaynakların bir dizisi. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Yazı tipi klasörünü ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | java.lang.String | TrueType yazı tiplerini içeren klasör. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Yazı tipi klasörünü ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType yazı tiplerini içeren klasörler. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Yazı tipi kaynaklarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | TrueType yazı tiplerini içeren kaynakların bir dizisi. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Verilen orijinal yazı tipi adı için yazı tipi ikame adları.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| originalFontName | java.lang.String | Orijinal yazı tipi adı. |
| substituteFontNames | java.lang.String[] | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarının listesi. |

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

