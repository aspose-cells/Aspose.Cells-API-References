---
title: "TxtSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "CSV/sekme sınırlı/diğer metin formatları için kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

CSV/sekme sınırlı/diğer metin formatları için kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Metin dosyası kaydetme seçeneklerini oluşturur. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Metin dosyası kaydetme seçeneklerini oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Her alan için her zaman '\"' eklenip eklenmeyeceğini gösterir. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getEncoding()](#getEncoding--) | Varsayılan kodlamayı alır. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExportAllSheets()](#getExportAllSheets--) | Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportArea()](#getExportArea--) | Dışa aktarılacak hücre aralığı. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Tek tırnak işaretinin, [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) true olduğunda bir hücrenin değerinin bir parçası olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [getFormatStrategy()](#getFormatStrategy--) | Hücre değerini dize olarak dışa aktarırken kullanılan biçim stratejisini alır. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getQuoteType()](#getQuoteType--) | Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını alır. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSeparator()](#getSeparator--) | Metin dosyasının karakter sınırlayıcısını alır. |
| [getSeparatorString()](#getSeparatorString--) | Ayırıcı olarak bir dize değeri alır. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | ms excel'in yaptığı gibi baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Her alan için her zaman '\"' eklenip eklenmeyeceğini gösterir. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Varsayılan kodlamayı ayarlar. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Dışa aktarılacak hücre aralığı. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Tek tırnak işaretinin, [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) true olduğunda bir hücrenin değerinin bir parçası olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini ayarlar. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setQuoteType(int value)](#setQuoteType-int-) | Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını ayarlar. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setSeparator(char value)](#setSeparator-char-) | Metin dosyasının karakter sınırlayıcısını ayarlar. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Ayırıcı olarak bir dize değeri ayarlar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | ms excel'in yaptığı gibi baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Metin dosyası kaydetme seçeneklerini oluşturur.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


Metin dosyası kaydetme seçeneklerini oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Dosya formatı. [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV) veya [SaveFormat.TSV](../../com.aspose.cells/saveformat\\#TSV) olmalıdır, aksi takdirde kaydedilen format otomatik olarak [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV) olarak ayarlanacaktır. |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Her alan için her zaman '\"' eklenip eklenmeyeceğini gösterir. Doğruysa tüm değerler tırnak içine alınır; Yanlışsa değerler yalnızca gerektiğinde (örneğin, değerler '\"', '\\\\n' veya ayırıcı karakter gibi özel karakterler içerdiğinde) tırnak içine alınır. Varsayılan değer yanlıştır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen QuoteType özelliğini kullanın. Bu özellik Ağustos 2012'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Varsayılan kodlamayı alır.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. Yanlışsa, sadece aktif sayfayı dışa aktarır, tıpkı MS Excel gibi.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Dışa aktarılacak hücre aralığı.

**Remarks**

Eğer dışa aktarılan alan belirtilmişse, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) etkisiz olacaktır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Bir hücrenin değeri içinde tek tırnak işaretinin dışa aktarılıp aktarılmayacağını, [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) true olduğunda gösterir. Varsayılan false'tur.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Hücre değerini dize olarak dışa aktarırken kullanılan biçim stratejisini alır.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false olduğundan, varsayılan olarak boş satırın içeriği boş olacaktır.

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
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını alır.

Bkz. [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Returns:**
int
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Metin dosyasının karakter sınırlayıcısını alır.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ayırıcı olarak bir dize değeri alır.

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


MS Excel'in yaptığı gibi, baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. Varsayılan true'tur.

**Remarks**

MS Excel'deki kurala benzer şekilde, özel bir stil içeren bir satır/sütun, hücre verisi olmasa bile boş olarak kabul edilmez. LightCells modunda kaydedilirken bu seçenek etkisiz olur. Kullanıcı, çıktının aralığını [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) uygulamasıyla ya da [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) belirterek kontrol etmelidir.

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan false'tur.

**Remarks**

LightCells modunda kaydedilirken ve [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) belirtilmemişse, bu seçenek etkisiz olur ve bir satır, [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) tarafından sağlanan son hücreye kadar genişletilir.

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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Her alan için her zaman '\"' eklenip eklenmeyeceğini gösterir. Doğruysa tüm değerler tırnak içine alınır; Yanlışsa değerler yalnızca gerektiğinde (örneğin, değerler '\"', '\\\\n' veya ayırıcı karakter gibi özel karakterler içerdiğinde) tırnak içine alınır. Varsayılan değer yanlıştır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen QuoteType özelliğini kullanın. Bu özellik Ağustos 2012'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Varsayılan kodlamayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. Yanlışsa, sadece aktif sayfayı dışa aktarır, tıpkı MS Excel gibi.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Dışa aktarılacak hücre aralığı.

**Remarks**

Eğer dışa aktarılan alan belirtilmişse, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) etkisiz olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Bir hücrenin değeri içinde tek tırnak işaretinin dışa aktarılıp aktarılmayacağını, [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) true olduğunda gösterir. Varsayılan false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Hücre değerini dize olarak dışa aktarırken biçim stratejisini ayarlar.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false olduğundan, varsayılan olarak boş satırın içeriği boş olacaktır.

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını ayarlar.

Bkz. [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Metin dosyasının karakter sınırlayıcısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Ayırıcı olarak bir dize değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


MS Excel'in yaptığı gibi, baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. Varsayılan true'tur.

**Remarks**

MS Excel'deki kurala benzer şekilde, özel bir stil içeren bir satır/sütun, hücre verisi olmasa bile boş olarak kabul edilmez. LightCells modunda kaydedilirken bu seçenek etkisiz olur. Kullanıcı, çıktının aralığını [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) uygulamasıyla ya da [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) belirterek kontrol etmelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan false'tur.

**Remarks**

LightCells modunda kaydedilirken ve [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) belirtilmemişse, bu seçenek etkisiz olur ve bir satır, [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) tarafından sağlanan son hücreye kadar genişletilir.

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

