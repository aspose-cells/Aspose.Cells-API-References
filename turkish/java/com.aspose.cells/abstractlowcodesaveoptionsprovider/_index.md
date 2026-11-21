---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "Birden fazla çıktı gerektiren süreçler için çoklu kaydetme seçenekleri sunan uygulama"
type: docs
url: /tr/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

Birden fazla çıktı gerektiren süreçler için birden fazla kaydetme seçeneği sağlamak amacıyla bir uygulamadır. Örneğin, [SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) özelliği, bölünmüş dosyaları kaydetmek için birden fazla hedef gerektirir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Mevcut bölünmüş parçanın işlenmesinden sonra kaynakları serbest bırakır. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Mevcut bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Mevcut bölünmüş parçanın işlenmesinden sonra kaynakları serbest bırakır.

**Remarks**

Varsayılan olarak bu yöntem, [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) tarafından belirtilen akışı doğrudan kapatır (eğer kaydetme seçenekleri bir Stream'i hedef olarak belirttiyse). Kullanıcı, gereksinimlerine ve [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-) uygulamasına göre kaynakların nasıl serbest bırakılacağını kontrol etmek için bu yöntemi geçersiz kılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Mevcut bölünmüş parça için kullanılan kaydetme seçenekleri. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Mevcut bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir. Null döndürmek, verilen parçayı atlamak anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
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

