---
title: "FileFormatUtil"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dosya formatı enumlarını dizeye veya dosya uzantısına ve geri dönüştürmek için yardımcı yöntemler sağlar."
type: docs
url: /tr/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Dosya formatı enumlarını dizeye veya dosya uzantısına ve geri dönüştürmek için yardımcı yöntemler sağlar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Bir dosyada depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Bir dosyada depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Bir dosya adı uzantısını SaveFormat değerine dönüştürür. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Dosya formatını kaydetme formatına dönüştürme. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Uzantı .xlt, .xltX, .xltm, .ots ise true döndürür. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Yükleme formatı enum değerini dosya uzantısına dönüştürür. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Mümkünse bir LoadFormat değerini SaveFormat değerine dönüştürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Kaydetme formatı enum değerini dosya uzantısına dönüştürür. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Mümkünse bir SaveFormat değerini LoadFormat değerine dönüştürür. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Akış |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | Şifreli ooxml dosyaları için parola. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Bir dosyada depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür.

**Remarks**

Yalnızca sihirli imzaya sahip bazı dosyaların kontrolünü destekler. Eğer sihirli imza yoksa, dosya formatını kesin olarak tespit edemeyiz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Bir dosyada depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür.

**Remarks**

Yalnızca sihirli imzaya sahip bazı dosyaların kontrolünü destekler. Eğer sihirli imza yoksa, dosya formatını kesin olarak tespit edemeyiz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| password | java.lang.String | Şifreli ooxml dosyaları için parola. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Bir dosya adı uzantısını SaveFormat değerine dönüştürür.

**Remarks**

Eğer uzantı tanınamazsa, [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN) döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extension | java.lang.String | Dosya uzantısı. Başında nokta olup olmadan olabilir. Büyük/küçük harfe duyarsız. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Dosya formatını kaydetme formatına dönüştürme.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Dosya formatı türü. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isTemplateFormat(String extension) {#isTemplateFormat-java.lang.String-}
```
public static boolean isTemplateFormat(String extension)
```


Uzantı .xlt, .xltX, .xltm, .ots ise true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Yükleme formatı enum değerini dosya uzantısına dönüştürür.

**Remarks**

Eğer dönüştürülemezse, null döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Yüklenen dosya formatı. |

**Returns:**
java.lang.String - Döndürülen uzantı, başında nokta bulunan küçük harfli bir dizedir.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Mümkünse bir LoadFormat değerini SaveFormat değerine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Yükleme formatı. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme formatı.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveFormatToExtension(int format) {#saveFormatToExtension-int-}
```
public static String saveFormatToExtension(int format)
```


Kaydetme formatı enum değerini dosya uzantısına dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme formatı. |

**Returns:**
java.lang.String - Döndürülen uzantı, başında nokta bulunan küçük harfli bir dizedir.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Mümkünse bir SaveFormat değerini LoadFormat değerine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme formatı. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Yükleme formatı
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(InputStream stream, String password) {#verifyPassword-java.io.InputStream-java.lang.String-}
```
public static boolean verifyPassword(InputStream stream, String password)
```


Bir akışta depolanan Excel'in formatı hakkında bilgileri algılar ve döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | Şifreli ooxml dosyaları için parola. |

**Returns:**
boolean - Parolanın düzeltilip düzeltilmediğini döndürür.
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

