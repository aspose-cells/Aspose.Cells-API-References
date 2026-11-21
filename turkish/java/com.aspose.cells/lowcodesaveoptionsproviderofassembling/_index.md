---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun SheetIndex veya SheetName SplitPartIndex gibi dizinler içerebilecek şekilde adlandırıldığı kaydetme seçeneklerini sağlamak için bir uygulama."
type: docs
url: /tr/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun (dizinler içerebilir) şu şekilde adlandırıldığı kaydetme seçeneklerini sağlamak için bir uygulama: [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(or SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Mevcut bölünmüş parçanın işlenmesinden sonra kaynakları serbest bırakır. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Dosya yolunun başlık kısmı (sayfa ve bölünmüş parça eklenmeden önce). |
| [getPathTail()](#getPathTail--) | Dosya yolunun son ek kısmı (sıra numaralarından sonra). |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Mevcut bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Çalışma sayfası dizini için önek. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Bölünmüş parçanın dizini için önek. |
| [getUseSheetName()](#getUseSheetName--) | Dosya yolunu sayfa indeksi yerine sayfa adıyla oluşturup oluşturmayacağını belirler. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Dosya yolunun başlık kısmı (sayfa ve bölünmüş parça eklenmeden önce). |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Dosya yolunun son ek kısmı (sıra numaralarından sonra). |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Çalışma sayfası dizini için önek. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Dosya yolunda kullanılan ve gerçek değeri arasındaki bölünmüş parçanın dizin ofseti([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Bölünmüş parçanın dizini için önek. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Dosya yolunu sayfa indeksi yerine sayfa adıyla oluşturup oluşturmayacağını belirler. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Sayfa indeksini veya adını her zaman dosya yoluna ekleyip eklemeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili önek dosya yoluna eklenmez.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Bölünmüş parça indeksini her zaman dosya yoluna ekleyip eklemeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek dosya yoluna eklenmez.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Dosya yolunun başlık kısmı (sayfa ve bölünmüş parça eklenmeden önce).

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Dosya yolunun son kısmı (sıra numaralarından sonra). Dosya adının uzantısını içermelidir.

**Returns:**
java.lang.String
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


[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon.

**Remarks**

Şablon belirtilmişse, oluşturulan örnek tüm ayarları ondan kopyalar ve çıktı dosyasını buna göre günceller.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Dosya yolunda kullanılan sayfa indeks ile gerçek değeri arasındaki fark ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Yalnızca [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false olduğunda etkili olur.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

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

Yalnızca bir bölünmüş parça varsa ve [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false ise, bu önek ve bölünmüş parça indeksi (0) sonuç dosya yoluna eklenmez.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Dosya yolunu sayfa indeksi yerine sayfa adıyla oluşturup oluşturmayacağını belirler. Varsayılan değer false'tur.

**Remarks**

Sayfa adı otomatik olarak yeniden oluşturulmayacaktır. Bu yüzden true olarak ayarlandığında, geçersiz dosya yolu veya adı oluşturabilecek özel bir sayfa adı olmadığından emin olun.

**Returns:**
boolean
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


Sayfa indeksini veya adını her zaman dosya yoluna ekleyip eklemeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili önek dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Bölünmüş parça indeksini her zaman dosya yoluna ekleyip eklemeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Dosya yolunun başlık kısmı (sayfa ve bölünmüş parça eklenmeden önce).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Dosya yolunun son kısmı (sıra numaralarından sonra). Dosya adının uzantısını içermelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) içinde kaydetme seçenekleri örneği oluşturmak için şablon.

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

**Remarks**

Yalnızca [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Çalışma sayfası dizini için önek.

**Remarks**

Yalnızca bir çalışma sayfası varsa ve [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false ise, bu önek ve sayfa indeksi (veya adı) sonuç dosya yoluna eklenmez.

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

Yalnızca bir bölünmüş parça varsa ve [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false ise, bu önek ve bölünmüş parça indeksi (0) sonuç dosya yoluna eklenmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Dosya yolunu sayfa indeksi yerine sayfa adıyla oluşturup oluşturmayacağını belirler. Varsayılan değer false'tur.

**Remarks**

Sayfa adı otomatik olarak yeniden oluşturulmayacaktır. Bu yüzden true olarak ayarlandığında, geçersiz dosya yolu veya adı oluşturabilecek özel bir sayfa adı olmadığından emin olun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

