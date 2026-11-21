---
title: "LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Düşük kodlu şekilde html kaydetme seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Düşük kodlu şekilde html kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | HTML kaydetmek için genel seçenekler. |
| [getOutputFile()](#getOutputFile--) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır. |
| [getOutputStream()](#getOutputStream--) | Oluşturulan verileri yazmak için akışı alır. |
| [getSaveFormat()](#getSaveFormat--) | Elektronik tablonun formatını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | HTML kaydetmek için genel seçenekler. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) ayarlar. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Oluşturulan verileri yazmak için akışı ayarlar. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Elektronik tablonun formatını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


HTML kaydetmek için genel seçenekler.

**Remarks**

Bir [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) örneği belirtildiğinde, [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) üzerine yazılacaktır (daha önce belirtilmişse).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


Elektronik tablonun formatını alır.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Bu özelliği değiştirirken, [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) tarafından belirtilen kaydetme formatı göz ardı edilecektir (daha önce belirtilmişse).

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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


HTML kaydetmek için genel seçenekler.

**Remarks**

Bir [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) örneği belirtildiğinde, [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) üzerine yazılacaktır (daha önce belirtilmişse).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


Elektronik tablonun formatını ayarlar.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Bu özelliği değiştirirken, [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) tarafından belirtilen kaydetme formatı göz ardı edilecektir (daha önce belirtilmişse).

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

