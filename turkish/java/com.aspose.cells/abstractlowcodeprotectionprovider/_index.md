---
title: "AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "Koruma ayarlarını sağlamak için uygulama"
type: docs
url: /tr/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Koruma ayarlarını sağlamak için uygulama
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Elektronik tablo dosyasını açmak için şifreyi alır. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Belirtilen koruma türüyle çalışma kitabını korumak için şifreyi alır. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Çalışma kitabını korumak için koruma türünü alır. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Belirtilen çalışma sayfasını korumak için şifreyi alır. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Belirtilen çalışma sayfasını korumak için koruma türünü alır. |
| [getWritePassword()](#getWritePassword--) | Elektronik tablo dosyasını değiştirmek için şifreyi alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Elektronik tablo dosyasını açmak için şifreyi alır.

**Returns:**
java.lang.String - Elektronik tablo dosyasını açmak için şifre. Boş olması dosyanın açılması için koruma olmadığını gösterir.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Belirtilen koruma türüyle çalışma kitabını korumak için şifreyi alır.

**Returns:**
java.lang.String - Çalışma kitabını korumak için şifre.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Çalışma kitabını korumak için koruma türünü alır.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Çalışma kitabını korumak için koruma türü. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) çalışma kitabı için koruma olmadığını ifade eder.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Belirtilen çalışma sayfasını korumak için şifreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Belirtilen çalışma sayfasını korumak için şifre.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Belirtilen çalışma sayfasını korumak için koruma türünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Belirtilen çalışma sayfasını korumak için koruma türü. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) çalışma sayfası için koruma olmadığını ifade eder.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Elektronik tablo dosyasını değiştirmek için şifreyi alır.

**Returns:**
java.lang.String - Elektronik tablo dosyasını değiştirmek için şifre. Boş, dosyanın değiştirilmesi için koruma olmadığını gösterir.
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

