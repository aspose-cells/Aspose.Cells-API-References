---
title: "DbfSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "dbf dosyasını kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/java/com.aspose.cells/dbfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class DbfSaveOptions extends SaveOptions
```

dbf dosyasını kaydetme seçeneklerini temsil eder
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DbfSaveOptions()](#DbfSaveOptions--) | .dbf dosyasını kaydetme seçenekleri. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExportAsString()](#getExportAsString--) | Dizgi değeri olarak dışa aktarmayı gösterir |
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
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Dizgi değeri olarak dışa aktarmayı gösterir |
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
### DbfSaveOptions() {#DbfSaveOptions--}
```
public DbfSaveOptions()
```


.dbf dosyasını kaydetme seçenekleri.

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
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Dizgi değeri olarak dışa aktarmayı gösterir

**Returns:**
boolean
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

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Dizgi değeri olarak dışa aktarmayı gösterir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

