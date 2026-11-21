---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "Birden fazla girdi (örneğin şablon dosyaları) kullanan süreçler için birden çok yükleme seçeneği sağlamak amacıyla bir uygulama."
type: docs
url: /tr/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Birden fazla girdi (örneğin şablon dosyaları) kullanan süreçler için çoklu yükleme seçenekleri sunan uygulama.

**Remarks**

Örneğin, [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) özelliği birleştirmek için birden çok şablon dosyası gerektirir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Girişin şu anda işlenen kısmı işlendikten sonra kaynakları serbest bırakır. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Şu anda işlenen kısmın verilerini yüklemek için kullanılacak yükleme seçeneklerini alır. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Daha fazla girdi olup olmadığını kontrol eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Girişin şu anda işlenen kısmı işlendikten sonra kaynakları serbest bırakır.

**Remarks**

Varsayılan olarak bu yöntem, [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) tarafından belirtilen akışı doğrudan kapatır (yükleme seçenekleri bir Stream'i kaynak olarak belirttiyse). Kullanıcı, gereksinimlerine ve [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--) uygulamasına göre kaynakları nasıl serbest bırakacağını kontrol etmek için bu yöntemi geçersiz kılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Şu anda bölünmüş parça için kullanılan yükleme seçenekleri. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Şu anda işlenen kısmın verilerini yüklemek için kullanılacak yükleme seçeneklerini alır.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Daha fazla girdi olup olmadığını kontrol eder.

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

