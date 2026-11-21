---
title: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Düşük kodlu şekilde pdf kaydetme seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

Düşük kodlu şekilde pdf kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır. |
| [getOutputStream()](#getOutputStream--) | Oluşturulan verileri yazmak için akışı alır. |
| [getPdfOptions()](#getPdfOptions--) | Pdf dosyasını kaydetmek için seçenekler. |
| [getSaveFormat()](#getSaveFormat--) | Çıktı için kaydetme biçimi. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) ayarlar. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Oluşturulan verileri yazmak için akışı ayarlar. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | Pdf dosyasını kaydetmek için seçenekler. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Çıktı için kaydetme biçimi. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


Pdf dosyasını kaydetmek için seçenekler.

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Çıktı için kaydetme biçimi. PDF'ye dönüştürmek için yalnızca [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF) olabilir.

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


Pdf dosyasını kaydetmek için seçenekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Çıktı için kaydetme biçimi. PDF'ye dönüştürmek için yalnızca [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF) olabilir.

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

