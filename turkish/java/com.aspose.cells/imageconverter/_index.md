---
title: "ImageConverter"
second_title: "Aspose.Cells for Java API Referansı"
description: "Şablon dosyasını görüntülere dönüştürmek için dönüştürücü."
type: docs
url: /tr/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Şablon dosyasını görüntülere dönüştürmek için dönüştürücü.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Şablon dosyasını görüntülere dönüştürür |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Şablon dosyasını görüntülere dönüştürür |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Şablon dosyasını görüntülere dönüştürür. |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


Şablon dosyasını görüntülere dönüştürür

**Remarks**

Birden fazla sayfayı destekleyen (örneğin tiff) formatta görüntüye dönüştürürken, belirtilen [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) veya [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) doğrudan sonuç görüntüsü için kullanılacaktır.

Diğer görüntü türleri için, kaydetme seçenekleri çıktı olarak Stream belirttiyse, tüm sonuç görüntüler aynı Stream'e kaydedilir. Aksi takdirde, çıktı dosyaları kaydetme seçeneklerinde belirtilen çıktı dosyasından, sayfa numarası ve bölünme parçası eklenerek oluşturulur. Örneğin, belirtilen çıktı dosyası Image.png ise, oluşturulan görüntü dosyaları Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ... şeklinde olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Giriş ve yükleme seçenekleri |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Çıktı ve kaydetme seçenekleri |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Şablon dosyasını görüntülere dönüştürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Giriş ve yükleme seçenekleri |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Kaydetme seçenekleri. Çıktısı ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) veya [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) etkisizdir çünkü tüm çıktılar "provider" parametresiyle belirtilecektir. |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Oluşturulan görüntüleri kaydetmek için kaydetme seçeneklerinin sağlayıcısı |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Şablon dosyasını görüntülere dönüştürür.

**Remarks**

Çıktı dosyaları, sayfa sıra numarası ve bölünme parçası eklenerek belirtilen sonuç dosyasından oluşturulacaktır. Örneğin, belirtilen çıktı dosyası Image.png ise, oluşturulan görüntü dosyaları Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | java.lang.String | Görüntülere dönüştürülecek şablon dosyası. |
| resultFile | java.lang.String | Oluşturulan görüntüler için sonuç dosyası (ad deseni). |

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

