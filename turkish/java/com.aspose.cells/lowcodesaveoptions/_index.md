---
title: "LowCodeSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Düşük kodlu şekilde oluşturulan sonuçları kaydetme seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

Düşük kodlu şekilde oluşturulan sonuçları kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır. |
| [getOutputStream()](#getOutputStream--) | Oluşturulan verileri yazmak için akışı alır. |
| [getSaveFormat()](#getSaveFormat--) | Çıktı için kaydetme biçimini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) ayarlar. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Oluşturulan verileri yazmak için akışı ayarlar. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Çıktı için kaydetme biçimini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
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
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) yok sayılacaktır.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Oluşturulan verileri yazmak için akışı alır. Bu özelliği null dışındaki bir değerle ayarladığınızda, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) yok sayılacaktır.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Çıktı için kaydetme biçimini alır. Genel olarak, düşük kodlu şekilde belirli bir işlem için yalnızca bazı belirli biçimlere izin verilir. Lütfen ilgili işlem için doğru biçimi belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
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




### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) ayarlar. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) yok sayılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Oluşturulan verileri yazmak için akışı ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) yok sayılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Çıktı için kaydetme biçimini ayarlar. Genel olarak, düşük kodlu şekilde belirli bir işlem için yalnızca bazı belirli biçimlere izin verilir. Lütfen ilgili işlem için doğru biçimi belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

