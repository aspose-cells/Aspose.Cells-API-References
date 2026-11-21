---
title: "XlsbSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "xlsb dosyasını kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/xlsbsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class XlsbSaveOptions extends SaveOptions
```

xlsb dosyasını kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XlsbSaveOptions()](#XlsbSaveOptions--) | xlsb dosyası kaydetme seçenekleri oluşturur. |
| [XlsbSaveOptions(int saveFormat)](#XlsbSaveOptions-int-) | xlsb dosyası kaydetme seçenekleri oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCompressionType()](#getCompressionType--) | ooxml dosyası için sıkıştırma türünü alır. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExportAllColumnIndexes()](#getExportAllColumnIndexes--) | hücreler için tüm sütun indekslerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCompressionType(int value)](#setCompressionType-int-) | ooxml dosyası için sıkıştırma türünü ayarlar. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExportAllColumnIndexes(boolean value)](#setExportAllColumnIndexes-boolean-) | hücreler için tüm sütun indekslerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XlsbSaveOptions() {#XlsbSaveOptions--}
```
public XlsbSaveOptions()
```


xlsb dosyası kaydetme seçenekleri oluşturur.

### XlsbSaveOptions(int saveFormat) {#XlsbSaveOptions-int-}
```
public XlsbSaveOptions(int saveFormat)
```


xlsb dosyası kaydetme seçenekleri oluşturur.

**Remarks**

NOT: Bu yapıcı artık kullanımdan kaldırılmıştır. Bunun yerine lütfen XlsbSaveOptions() yapıcısını kullanın. Bu özellik, Ocak 2021'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme biçimi. xlsb olmalıdır. |

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

**Remarks**

Eğer klasör belirtilmemişse, varsayılan değeri [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)'dır. Eğer varsayılan değeri null veya boş ise, ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken önbellek dosyası kullanılmaz.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarını kontrol edip etmeyeceği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girdiğinizde, kesilir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Returns:**
boolean
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


ooxml dosyası için sıkıştırma türünü alır.

Bakınız [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Varsayılan değer OoxmlCompressionType.Level6'dır.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Returns:**
boolean
### getExportAllColumnIndexes() {#getExportAllColumnIndexes--}
```
public boolean getExportAllColumnIndexes()
```


hücreler için tüm sütun indekslerinin dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Varsayılan değer true'tır.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Kaydetme dosya formatını alır.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Akıllı sanat ayarının güncellenip güncellenmeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Shape.GetResultOfSmartArt() yöntemi çağrıldıktan ve önbelleğe alınmış şekiller şablon dosyasında mevcut olduğunda etkili olur.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Uyarı geri çağrısını alır.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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




### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

**Remarks**

Eğer klasör belirtilmemişse, varsayılan değeri [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)'dır. Eğer varsayılan değeri null veya boş ise, ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken önbellek dosyası kullanılmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarını kontrol edip etmeyeceği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girdiğinizde, kesilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


ooxml dosyası için sıkıştırma türünü ayarlar.

Bakınız [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Varsayılan değer OoxmlCompressionType.Level6'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportAllColumnIndexes(boolean value) {#setExportAllColumnIndexes-boolean-}
```
public void setExportAllColumnIndexes(boolean value)
```


hücreler için tüm sütun indekslerinin dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Akıllı sanat ayarının güncellenip güncellenmeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Shape.GetResultOfSmartArt() yöntemi çağrıldıktan ve önbelleğe alınmış şekiller şablon dosyasında mevcut olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Uyarı geri çağrısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

