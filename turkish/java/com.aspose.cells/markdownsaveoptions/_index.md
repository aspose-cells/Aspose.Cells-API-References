---
title: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Markdown için kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/markdownsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class MarkdownSaveOptions extends SaveOptions
```

Markdown için kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MarkdownSaveOptions()](#MarkdownSaveOptions--) | Markdown belgesini kaydetmek için seçenekler oluşturur |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignColumnPadding()](#getAlignColumnPadding--) | Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCalculateFormula()](#getCalculateFormula--) | Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getEncoding()](#getEncoding--) | Varsayılan kodlamayı alır. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--) | Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Görsellerin Markdown'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [getFormatStrategy()](#getFormatStrategy--) | Hücre değerini dize olarak dışa aktarırken kullanılan biçim stratejisini alır. |
| [getImageOptions()](#getImageOptions--) | Dışa aktarmadan önce ImageOrPrintOptions nesnesini al |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Çalışma kitabını hafif modda kaydetmek için hücre verilerini sağlayan Veri sağlayıcı. |
| [getLineSeparator()](#getLineSeparator--) | Satır ayırıcıyı alır. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--) | OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSheetSet()](#getSheetSet--) | Render edilecek sayfaları alır. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--) | Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. |
| [getStreamProvider()](#getStreamProvider--) | Nesneleri dışa aktarmak için IStreamProvider'ı alır. |
| [getTableHeaderType()](#getTableHeaderType--) | Tablonun başlığının nasıl ayarlandığını alır. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignColumnPadding(char value)](#setAlignColumnPadding-char-) | Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Varsayılan kodlamayı ayarlar. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExportHyperlinkAsReference(boolean value)](#setExportHyperlinkAsReference-boolean-) | Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Görsellerin Markdown'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini ayarlar. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Çalışma kitabını hafif modda kaydetmek için hücre verilerini sağlayan Veri sağlayıcı. |
| [setLineSeparator(String value)](#setLineSeparator-java.lang.String-) | Satır ayırıcıyı ayarlar. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setOfficeMathOutputType(int value)](#setOfficeMathOutputType-int-) | OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Render edilecek sayfaları ayarlar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSplitTablesByBlankRow(boolean value)](#setSplitTablesByBlankRow-boolean-) | Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Nesneleri dışa aktarmak için IStreamProvider'ı ayarlar. |
| [setTableHeaderType(int value)](#setTableHeaderType-int-) | Tablonun başlığının nasıl ayarlandığını belirler. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MarkdownSaveOptions() {#MarkdownSaveOptions--}
```
public MarkdownSaveOptions()
```


Markdown belgesini kaydetmek için seçenekler oluşturur

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
### getAlignColumnPadding() {#getAlignColumnPadding--}
```
public char getAlignColumnPadding()
```


Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriğini doldurarak hizalanır. Sütun hizalamasını devre dışı bırakmak için '\\0' olarak ayarlayın (varsayılan).

**Returns:**
char
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

**Remarks**

Eğer klasör belirtilmemişse, varsayılan değeri [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)'dır. Eğer varsayılan değeri null veya boş ise, ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken önbellek dosyası kullanılmaz.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
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
### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}
```
public boolean getExportHyperlinkAsReference()
```


Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Görsellerin Markdown'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. Varsayılan değer true'dur.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Dışa aktarmadan önce ImageOrPrintOptions nesnesini al

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Çalışma kitabını hafif modda kaydetmek için hücre verilerini sağlayan Veri sağlayıcı.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getLineSeparator() {#getLineSeparator--}
```
public String getLineSeparator()
```


Satır ayırıcıyı alır.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getOfficeMathOutputType() {#getOfficeMathOutputType--}
```
public int getOfficeMathOutputType()
```


OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür.

Bakınız [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Render edilecek sayfaları alır. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Bu ayar, [SheetRender](../../com.aspose.cells/sheetrender) içinde kullanıldığında yok sayılır.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}
```
public boolean getSplitTablesByBlankRow()
```


Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Nesneleri dışa aktarmak için IStreamProvider'ı alır. `null` ise, dışa aktarılan nesneler çıktı dosyasıyla aynı dizine kaydedilir.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableHeaderType() {#getTableHeaderType--}
```
public int getTableHeaderType()
```


Tablonun başlığının nasıl ayarlandığını alır.

Bakınız [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Returns:**
int
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




### setAlignColumnPadding(char value) {#setAlignColumnPadding-char-}
```
public void setAlignColumnPadding(char value)
```


Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriğini doldurarak hizalanır. Sütun hizalamasını devre dışı bırakmak için '\\0' olarak ayarlayın (varsayılan).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setExportHyperlinkAsReference(boolean value) {#setExportHyperlinkAsReference-boolean-}
```
public void setExportHyperlinkAsReference(boolean value)
```


Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Görsellerin Markdown'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. Varsayılan değer true'dur.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

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

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Çalışma kitabını hafif modda kaydetmek için hücre verilerini sağlayan Veri sağlayıcı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setLineSeparator(String value) {#setLineSeparator-java.lang.String-}
```
public void setLineSeparator(String value)
```


Satır ayırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

### setOfficeMathOutputType(int value) {#setOfficeMathOutputType-int-}
```
public void setOfficeMathOutputType(int value)
```


OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür.

Bakınız [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Render edilecek sayfaları ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Bu ayar, [SheetRender](../../com.aspose.cells/sheetrender) içinde kullanıldığında yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setSplitTablesByBlankRow(boolean value) {#setSplitTablesByBlankRow-boolean-}
```
public void setSplitTablesByBlankRow(boolean value)
```


Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Nesneleri dışa aktarmak için IStreamProvider'ı ayarlar. `null` ise, dışa aktarılan nesneler çıktı dosyasıyla aynı dizine kaydedilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableHeaderType(int value) {#setTableHeaderType-int-}
```
public void setTableHeaderType(int value)
```


Tablonun başlığının nasıl ayarlandığını belirler.

Bakınız [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

