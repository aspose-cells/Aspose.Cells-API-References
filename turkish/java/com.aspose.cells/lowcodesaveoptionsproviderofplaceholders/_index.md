---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dosya parçalarını dosyalara kaydeden ve ortaya çıkan dosyanın yolunun yer tutucularla tanımlandığı kaydetme seçeneklerini sağlamak için uygulama."
type: docs
url: /tr/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Dosya parçalarını dosyalara kaydeden ve ortaya çıkan dosyanın yolunun yer tutucularla tanımlandığı kaydetme seçeneklerini sağlamak için uygulama.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Belirtilen şablonlara göre kaydetme seçenekleri sağlayacak bir örnek oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Mevcut bölünmüş parçanın işlenmesinden sonra kaynakları serbest bırakır. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Mevcut bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Çalışma sayfası dizini için önek. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Çalışma sayfası dizini için önek. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Bölünmüş parçanın dizini için önek. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Çalışma sayfası dizini için önek. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Çalışma sayfası dizini için önek. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Bölünmüş parçanın dizini için önek. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Belirtilen şablonlara göre kaydetme seçenekleri sağlayacak bir örnek oluşturur.

**Remarks**

Dosya yolu şablonunda desteklenen yer tutucular:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pathTemplate | java.lang.String | Sonuç dosya yolunun şablonu. |

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

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Sayfa indeksi veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir sayfa olduğunda, sayfa indeksi ve adı ile ilgili önek ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) dosya yoluna eklenmez.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) dosya yoluna eklenmez.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Mevcut bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon.

**Remarks**

Şablon belirtilmişse, oluşturulan örnek tüm ayarları ondan kopyalar ve çıktı dosyasını buna göre günceller.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Bölünmüş parçanın dizini için önek.

**Remarks**

Yalnızca bir bölünmüş parça varsa ve [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) false ise, bu önek ve bölünmüş parça indeksi (0) sonuç dosya yoluna eklenmez.

**Returns:**
java.lang.String
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Sayfa indeksi veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir sayfa olduğunda, sayfa indeksi ve adı ile ilgili önek ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon.

**Remarks**

Şablon belirtilmişse, oluşturulan örnek tüm ayarları ondan kopyalar ve çıktı dosyasını buna göre günceller.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Bölünmüş parçanın dizini için önek.

**Remarks**

Yalnızca bir bölünmüş parça varsa ve [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) false ise, bu önek ve bölünmüş parça indeksi (0) sonuç dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

