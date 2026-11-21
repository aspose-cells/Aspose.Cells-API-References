---
title: "PdfSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "PDF dosyasını kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

PDF dosyasını kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | PDF dosyasını kaydetmek için seçenekleri oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getBookmark()](#getBookmark--) | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) nesnesini alır. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCalculateFormula()](#getCalculateFormula--) | PDF dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCompliance()](#getCompliance--) | Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getCreatedTime()](#getCreatedTime--) | PDF belgesinin oluşturulma zamanını alır. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | PDF dosyasına [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) öğelerinin nasıl dışa aktarılacağını belirleyen bir değeri alır. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Renderleme sırasında özel ayarları alır. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Varsayılan düzenleme dilini alır. |
| [getDefaultFont()](#getDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Excel'deki Ole nesneleri için ekin gömülüp gömülmeyeceğini belirtir. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True type yazı tiplerini gömmek için true. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Emf meta dosyasını işleme ayarı. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Belge yapısının dışa aktarılıp aktarılmayacağını belirtir. |
| [getFontEncoding()](#getFontEncoding--) | PDF'de gömülü yazı tipi kodlamasını alır. |
| [getGridlineColor()](#getGridlineColor--) | Izgara çizgisi rengini alır. |
| [getGridlineType()](#getGridlineType--) | Izgara çizgisi tipini alır. |
| [getIgnoreError()](#getIgnoreError--) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. |
| [getImageType()](#getImageType--) | Grafik ve şekil dönüştürülürken görüntü türünü temsil eder. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getOptimizationType()](#getOptimizationType--) | PDF optimizasyon türünü alır. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [getPageCount()](#getPageCount--) | Kaydedilecek sayfa sayısını alır. |
| [getPageIndex()](#getPageIndex--) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [getPdfCompression()](#getPdfCompression--) | Sıkıştırma algoritmasını belirtir. |
| [getPrintingPageType()](#getPrintingPageType--) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [getProducer()](#getProducer--) | Oluşturulan PDF belgesinin üreticisini alır. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Uygulanacak Excel'e özgü renderleme davranışlarını alır. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSecurityOptions()](#getSecurityOptions--) | xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın. |
| [getSheetSet()](#getSheetSet--) | Render edilecek sayfaları alır. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getTextCrossType()](#getTextCrossType--) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü alır. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [getWatermark()](#getWatermark--) | Çıktıya eklenecek filigranı alır. |
| [getZoomBehavior()](#getZoomBehavior--) | Oluşturulan PDF belgesi açıldığında ilk görüntüleme modunu alır. |
| [getZoomFactor()](#getZoomFactor--) | Zoom davranışı [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR) olduğunda kullanılan yakınlaştırma yüzdesini alır. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) nesnesini ayarlar. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | PDF dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCompliance(int value)](#setCompliance-int-) | Çıktı belgeleri için PDF standartları uyumluluk seviyesini ayarlar. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | PDF belgesinin oluşturulma zamanını ayarlar. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) öğelerinin PDF dosyasına nasıl dışa aktarılacağını belirleyen bir değeri ayarlar. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Renderleme sırasında özel ayarları belirler. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Varsayılan düzenleme dilini ayarlar. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Excel'deki Ole nesneleri için ekin gömülüp gömülmeyeceğini belirtir. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | True type yazı tiplerini gömmek için true. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Emf meta dosyasını işleme ayarı. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Belge yapısının dışa aktarılıp aktarılmayacağını belirtir. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | PDF'de gömülü yazı tipi kodlamasını ayarlar. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Kılavuz çizgi rengini ayarlar. |
| [setGridlineType(int value)](#setGridlineType-int-) | Kılavuz çizgi tipini ayarlar. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Yeniden örneklenen görüntülerin istenen PPI (inç başına piksel) ve jpeg kalitesini ayarlar. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Grafik ve şekil dönüştürülürken görüntü türünü temsil eder. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | PDF optimizasyon türünü ayarlar. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [setPageCount(int value)](#setPageCount-int-) | Kaydedilecek sayfa sayısını ayarlar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Sıkıştırma algoritmasını belirtir. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Oluşturulan PDF belgesinin üreticisini ayarlar. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Uygulanacak Excel'e özgü renderleme davranışlarını ayarlar. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Render edilecek sayfaları ayarlar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü ayarlar. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Çıktıya filigran ekler. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Oluşturulan PDF belgesi açıldığında başlangıç görünüm modunu ayarlar. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Zoom yüzdesini, [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR) olduğunda ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


PDF dosyasını kaydetmek için seçenekleri oluşturur.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. pagesetup'ın kağıt boyutu genişliği göz ardı edilir ve pagesetup'ın diğer ayarları hâlâ etkili olur.

**Returns:**
boolean
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) nesnesini alır.

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
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


PDF dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

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
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir.

**Remarks**

Varsayılan değer true'dur. Bu özelliği devre dışı bırakmak daha iyi performans sağlayabilir. Ancak metin/karakterin varsayılan veya belirtilen yazı tipi render için kullanılamadığında, oluşturulan pdf'de okunamayan karakterler (örneğin blok) ortaya çıkabilir. Böyle bir durumda kullanıcı bu özelliği true olarak tutmalı, böylece alternatif bir yazı tipi aranıp metni render etmek için kullanılabilir;

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipi kullanılarak bu karakterler gösterilmeye çalışılır.

**Remarks**

Varsayılan true'dur.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır.

Bakınız [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Varsayılan Pdf17'dir.

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
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


PDF belgesinin oluşturulma zamanını alır.

**Remarks**

Ayarlanmamışsa, PDF oluşturulma zamanı kullanılacaktır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


PDF dosyasına dışa aktarılırken [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) koleksiyonunun nasıl işleneceğini belirleyen bir değer alır. Varsayılan değer None'dur.

Bakınız [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Renderleme sırasında özel ayarları alır.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Varsayılan düzenleme dilini alır.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

**Returns:**
java.lang.String
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir.

**Remarks**

Yanlış (false) ise, başlık çubuğu PDF dosyasının adını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Excel'deki Ole nesneleri için ekin gömülüp gömülmeyeceğini belirtir.

**Remarks**

Varsayılan değer false'tur. PDF/A uyumluluğu ayarlandığında veya PDF şifrelemesi etkinleştirildiğinde değer false olmalıdır.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True (doğru) olarak TrueType yazı tipleri gömülür. Yalnızca ASCII karakterleri 32-127'yi etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A-1a, PDF/A-1b standartları için yazı tipleri her zaman gömülür. Varsayılan true'tur.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Emf meta dosyasını işleme ayarı.

Bakınız [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

\"EMF+ Dual\" olarak tanımlanan EMF metafileleri hem EMF+ kayıtları hem de EMF kayıtları içerebilir. Her iki kayıt türü de görüntüyü renderlemek için kullanılabilir, yalnızca EMF+ kayıtları veya yalnızca EMF kayıtları kullanılabilir. [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) ayarlandığında, sayfaya renderleme sırasında EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)'dır.

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Returns:**
boolean
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Belge yapısının dışa aktarılıp aktarılmayacağını belirtir.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


PDF'de gömülü yazı tipi kodlamasını alır.

Bakınız [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Varsayılan değer [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\\#IDENTITY)'dir.

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Izgara çizgisi rengini alır.

**Remarks**

Kaynak dosyadaki kılavuz çizgi renk ayarlarını yok sayacaktır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Izgara çizgisi tipini alır.

Bakınız [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Varsayılan Dotted tipidir.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik renderleme vb. hatalar olabilir.

**Returns:**
boolean
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Grafik ve şekil dönüştürülürken görüntü türünü temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Chart ve Shape her zaman vektör öğeleri (ör. nokta, çizgi) olarak işlenir, böylece render kalitesi artar. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacak, ancak pagesetup'ın diğer ayarları hâlâ etkili olacaktır.

**Returns:**
boolean
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


PDF optimizasyon türünü alır.

Bakınız [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Varsayılan değer [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\\#STANDARD)'dir.

**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir.

**Remarks**

Varsayılan true'dur.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Kaydedilecek sayfa sayısını alır.

**Remarks**

Varsayılan, System.Int32.MaxValue'dir ve bu, tüm sayfaların işleneceği anlamına gelir..

**Example**

Aşağıdaki örnek, bir Microsoft Excel dosyasındaki sayfa aralığını (3 ve 4) PDF'ye nasıl işleneceğini gösterir.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır.

**Remarks**

Varsayılan 0'dır.

**Example**

Aşağıdaki örnek, bir Microsoft Excel dosyasındaki sayfa aralığını (3 ve 4) PDF'ye nasıl işleneceğini gösterir.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Sıkıştırma algoritmasını belirtir.

Bakınız [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Hangi sayfaların yazdırılmayacağını gösterir.

Bakınız [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Sayfadaki içerik seyrek ise, çıktı pdf dosyasında bazı sayfalar tamamen boş olacaktır. Bu boş sayfaları istemiyorsanız, bu seçeneği kullanarak onları atlayabilirsiniz.

**Example**

Aşağıdaki kod, hücre arka planı, kenarlıklar gibi yalnızca stil içeriği içeren boş sayfaları veya sayfaları atlar.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getProducer() {#getProducer--}
```
public String getProducer()
```


Oluşturulan PDF belgesinin üreticisini alır.

**Remarks**

Değer null ise veya geçerli bir LICENSE ayarlanmamışsa, Aspose.Cells vVERSION dizesi kullanılacaktır.

**Returns:**
java.lang.String
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Uygulanacak Excel'e özgü renderleme davranışlarını alır.

Bakınız [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Varsayılan değer [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL)'dır.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Kaydetme dosya formatını alır.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.

**Example**

Aşağıdaki kod, çıktı PDF'si için yüksek çözünürlük baskı iznini ayarlar.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Render edilecek sayfaları alır. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

Aşağıdaki kod yalnızca aktif sayfayı pdf'ye işler.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

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
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü alır.

Bakınız [TextCrossType](../../com.aspose.cells/textcrosstype).

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
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Çıktıya eklenecek filigranı alır.

**Example**

Aşağıdaki kod, çıktı PDF'sine filigran ekler.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Oluşturulan PDF belgesi açıldığında başlangıç görünüm modunu alır. Varsayılan değer [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\\#NONE)'dir.

Bakınız [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Zoom davranışı [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR) olduğunda kullanılan yakınlaştırma yüzdesini alır.

**Remarks**

Bu özellik, [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR) olmadıkça yok sayılır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur. Önce hücre yazı tipi için Workbook ve PdfSaveOption/sistem'in varsayılan yazı tipini deneyeceğiz.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. pagesetup'ın kağıt boyutu genişliği göz ardı edilir ve pagesetup'ın diğer ayarları hâlâ etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) nesnesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

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


PDF dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

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

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir.

**Remarks**

Varsayılan değer true'dur. Bu özelliği devre dışı bırakmak daha iyi performans sağlayabilir. Ancak metin/karakterin varsayılan veya belirtilen yazı tipi render için kullanılamadığında, oluşturulan pdf'de okunamayan karakterler (örneğin blok) ortaya çıkabilir. Böyle bir durumda kullanıcı bu özelliği true olarak tutmalı, böylece alternatif bir yazı tipi aranıp metni render etmek için kullanılabilir;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipi kullanılarak bu karakterler gösterilmeye çalışılır.

**Remarks**

Varsayılan true'dur.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Çıktı belgeleri için PDF standartları uyumluluk seviyesini ayarlar.

Bakınız [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Varsayılan Pdf17'dir.

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

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


PDF belgesinin oluşturulma zamanını ayarlar.

**Remarks**

Ayarlanmamışsa, PDF oluşturulma zamanı kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


PDF dosyasına dışa aktarılırken [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) koleksiyonunun nasıl işleneceğini belirleyen bir değer ayarlar. Varsayılan değer None'dur.

Bakınız [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Renderleme sırasında özel ayarları belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Varsayılan düzenleme dilini ayarlar.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir.

**Remarks**

Yanlış (false) ise, başlık çubuğu PDF dosyasının adını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Excel'deki Ole nesneleri için ekin gömülüp gömülmeyeceğini belirtir.

**Remarks**

Varsayılan değer false'tur. PDF/A uyumluluğu ayarlandığında veya PDF şifrelemesi etkinleştirildiğinde değer false olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True (doğru) olarak TrueType yazı tipleri gömülür. Yalnızca ASCII karakterleri 32-127'yi etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A-1a, PDF/A-1b standartları için yazı tipleri her zaman gömülür. Varsayılan true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Emf meta dosyasını işleme ayarı.

Bakınız [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

\"EMF+ Dual\" olarak tanımlanan EMF metafileleri hem EMF+ kayıtları hem de EMF kayıtları içerebilir. Her iki kayıt türü de görüntüyü renderlemek için kullanılabilir, yalnızca EMF+ kayıtları veya yalnızca EMF kayıtları kullanılabilir. [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) ayarlandığında, sayfaya renderleme sırasında EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Belge yapısının dışa aktarılıp aktarılmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


PDF'de gömülü yazı tipi kodlamasını ayarlar.

Bakınız [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Varsayılan değer [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\\#IDENTITY)'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur. Önce hücre yazı tipi için Workbook ve PdfSaveOption/sistem'in varsayılan yazı tipini deneyeceğiz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Kılavuz çizgi rengini ayarlar.

**Remarks**

Kaynak dosyadaki kılavuz çizgi renk ayarlarını yok sayacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Kılavuz çizgi tipini ayarlar.

Bakınız [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Varsayılan Dotted tipidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik renderleme vb. hatalar olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Yeniden örnekleme görüntülerinin istenen PPI (inç başına piksel) ve jpeg kalitesini ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI'den (inç başına piksel) büyük olan görüntüler yeniden örneklenir.

**Example**

Aşağıdaki kod, çıktı PDF'sindeki görüntüler için istenen PPI'yi 96 ve jpeg kalitesini 80 olarak ayarlar.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredPPI | int | İstenen inç başına piksel. 220 yüksek kalite. 150 ekran kalitesi. 96 e-posta kalitesi. |
| jpegQuality | int | 0 - %100 JPEG kalitesi. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Grafik ve şekil dönüştürülürken görüntü türünü temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Chart ve Shape her zaman vektör öğeleri (ör. nokta, çizgi) olarak işlenir, böylece render kalitesi artar. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacak, ancak pagesetup'ın diğer ayarları hâlâ etkili olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


PDF optimizasyon türünü ayarlar.

Bakınız [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Varsayılan değer [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\\#STANDARD)'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir.

**Remarks**

Varsayılan true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Kaydedilecek sayfa sayısını ayarlar.

**Remarks**

Varsayılan, System.Int32.MaxValue'dir ve bu, tüm sayfaların işleneceği anlamına gelir..

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Kaydedilecek ilk sayfanın 0 tabanlı indeksini ayarlar.

**Remarks**

Varsayılan 0'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Sıkıştırma algoritmasını belirtir.

Bakınız [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Hangi sayfaların yazdırılmayacağını gösterir.

Bakınız [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Sayfadaki içerik seyrek ise, çıktı pdf dosyasında bazı sayfalar tamamen boş olacaktır. Bu boş sayfaları istemiyorsanız, bu seçeneği kullanarak onları atlayabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Oluşturulan PDF belgesinin üreticisini ayarlar.

**Remarks**

Değer null ise veya geçerli bir LICENSE ayarlanmamışsa, Aspose.Cells vVERSION dizesi kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Uygulanacak Excel'e özgü renderleme davranışlarını ayarlar.

Bakınız [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Varsayılan değer [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL)'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Render edilecek sayfaları ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

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

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü ayarlar.

Bakınız [TextCrossType](../../com.aspose.cells/textcrosstype).

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Çıktıya filigran ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Oluşturulan PDF belgesi açıldığında başlangıç görünüm modunu ayarlar. Varsayılan değer [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE) dir.

Bakınız [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Zoom yüzdesini, [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR) olduğunda ayarlar.

**Remarks**

Bu özellik, [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR) olmadıkça yok sayılır.

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

