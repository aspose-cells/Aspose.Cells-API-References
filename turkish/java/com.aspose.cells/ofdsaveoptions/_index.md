---
title: "OfdSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "OFDOpen Sabit-düzen Belge dosyasını kaydetmek için seçenekleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/ofdsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class OfdSaveOptions extends PaginatedSaveOptions
```

OFD (Open Fixed-layout Document) dosyasını kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [OfdSaveOptions()](#OfdSaveOptions--) | OFD dosyasını kaydetmek için seçenekleri oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Renderleme sırasında özel ayarları alır. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Varsayılan düzenleme dilini alır. |
| [getDefaultFont()](#getDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Emf meta dosyasını işleme ayarı. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getGridlineColor()](#getGridlineColor--) | Izgara çizgisi rengini alır. |
| [getGridlineType()](#getGridlineType--) | Izgara çizgisi tipini alır. |
| [getIgnoreError()](#getIgnoreError--) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [getPageCount()](#getPageCount--) | Kaydedilecek sayfa sayısını alır. |
| [getPageIndex()](#getPageIndex--) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [getPrintingPageType()](#getPrintingPageType--) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Uygulanacak Excel'e özgü renderleme davranışlarını alır. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSheetSet()](#getSheetSet--) | Render edilecek sayfaları alır. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getTextCrossType()](#getTextCrossType--) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü alır. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Renderleme sırasında özel ayarları belirler. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Varsayılan düzenleme dilini ayarlar. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Emf meta dosyasını işleme ayarı. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Kılavuz çizgi rengini ayarlar. |
| [setGridlineType(int value)](#setGridlineType-int-) | Kılavuz çizgi tipini ayarlar. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [setPageCount(int value)](#setPageCount-int-) | Kaydedilecek sayfa sayısını ayarlar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Uygulanacak Excel'e özgü renderleme davranışlarını ayarlar. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Render edilecek sayfaları ayarlar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü ayarlar. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OfdSaveOptions() {#OfdSaveOptions--}
```
public OfdSaveOptions()
```


OFD dosyasını kaydetmek için seçenekleri oluşturur.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
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
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
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

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

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

