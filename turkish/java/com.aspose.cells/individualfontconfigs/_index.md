---
title: "IndividualFontConfigs"
second_title: "Aspose.Cells for Java API Referansı"
description: "Her bir nesne için yazı tipi yapılandırmaları."
type: docs
url: /tr/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Her bir [Workbook](../../com.aspose.cells/workbook) nesnesi için yazı tipi yapılandırmaları.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Kaynakların listesini içeren dizinin bir kopyasını alır. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi yedek adlarını içeren bir dizi döndürür. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Yazı tiplerinin yalnızca kaynaklarını ayarlar. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Yazı tipi klasörünü ayarlar |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Yazı tipi klasörlerini ayarlar. |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Yazı tipi kaynaklarını ayarlar. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Belirli bir orijinal yazı tipi adı için yazı tipi yedek adlarını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


Yapıcı.

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
### getFontSources() {#getFontSources--}
```
public FontSourceBase[] getFontSources()
```


Kaynakların listesini içeren dizinin bir kopyasını alır.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public void setFontFolder(String fontFolder, boolean recursive)
```


Yazı tipi klasörünü ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | java.lang.String | TrueType yazı tiplerini içeren klasör. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Yazı tipi klasörlerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType yazı tiplerini içeren klasörler. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Yazı tipi kaynaklarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | TrueType yazı tiplerini içeren kaynakların bir dizisi. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Belirli bir orijinal yazı tipi adı için yazı tipi yedek adlarını ayarlar.

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

