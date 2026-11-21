---
title: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Düşük kodlu şekilde resim kaydetme seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Düşük kodlu şekilde resim kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Görüntüleri işlemek için seçenekler. |
| [getOutputFile()](#getOutputFile--) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır. |
| [getOutputStream()](#getOutputStream--) | Oluşturulan verileri yazmak için akışı alır. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme biçimini alır. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Görüntüleri işlemek için seçenekler. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) ayarlar. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Oluşturulan verileri yazmak için akışı ayarlar. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Kaydetme biçimini ayarlar. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Görüntüleri işlemek için seçenekler.

**Remarks**

Bir [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) örneği belirtildiğinde, [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) önce belirtilmişse üzerine yazılacaktır.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


Kaydetme biçimini alır.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Eğer [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) belirtilmişse, bu özelliğin ayarlanması aynı zamanda [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) değerini de değiştirecektir.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı.

**Remarks**

Bu örnek tarafından belirtilen çıktı([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) veya [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) bu özellik belirtildiğinde etkisiz olacaktır. Bunun yerine, her oluşturulan görüntünün çıktısı sağlayıcı tarafından belirlenecektir.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


Görüntüleri işlemek için seçenekler.

**Remarks**

Bir [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) örneği belirtildiğinde, [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) önce belirtilmişse üzerine yazılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


Kaydetme biçimini ayarlar.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Eğer [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) belirtilmişse, bu özelliğin ayarlanması aynı zamanda [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) değerini de değiştirecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı.

**Remarks**

Bu örnek tarafından belirtilen çıktı([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) veya [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) bu özellik belirtildiğinde etkisiz olacaktır. Bunun yerine, her oluşturulan görüntünün çıktısı sağlayıcı tarafından belirlenecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

