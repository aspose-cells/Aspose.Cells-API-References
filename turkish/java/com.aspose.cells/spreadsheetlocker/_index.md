---
title: "SpreadsheetLocker"
second_title: "Aspose.Cells for Java API Referansı"
description: "Elektronik tablo dosyasını kilitlemek için düşük kodlu API."
type: docs
url: /tr/java/com.aspose.cells/spreadsheetlocker/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetLocker
```

Elektronik tablo dosyasını kilitlemek için düşük kodlu API.

**Example**

```
         SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| [process(String templateFile, String resultFile, String openPassword, String writePassword)](#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)
```


Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Giriş ve yükleme seçenekleri |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Çıktı ve kaydetme seçenekleri |
| provider | [AbstractLowCodeProtectionProvider](../../com.aspose.cells/abstractlowcodeprotectionprovider) | Koruma ayarlarını sağlamak için uygulama |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)
```


Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Giriş ve yükleme seçenekleri |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Çıktı ve kaydetme seçenekleri |
| openPassword | java.lang.String | Dosya şifrelemesi için parola |
| writePassword | java.lang.String | Elektronik tabloyu değiştirme koruması şifresi |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)
```


Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Giriş ve yükleme seçenekleri |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Çıktı ve kaydetme seçenekleri |
| openPassword | java.lang.String | Dosya şifrelemesi için parola |
| writePassword | java.lang.String | Elektronik tabloyu değiştirme koruması şifresi |
| workbookPassword | java.lang.String | Çalışma kitabının koruması için şifre |
| workbookType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Çalışma kitabını korumak için koruma türü |

### process(String templateFile, String resultFile, String openPassword, String writePassword) {#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile, String openPassword, String writePassword)
```


Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | java.lang.String | Kilitlenecek şablon dosyası |
| resultFile | java.lang.String | Ortaya çıkan dosya |
| openPassword | java.lang.String | Dosya şifrelemesi için parola |
| writePassword | java.lang.String | Elektronik tabloyu değiştirme koruması şifresi |

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

