---
title: "EbookLoadOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir e-kitap dosyası içe aktarılırken seçenekleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

Bir e-kitap dosyası içe aktarılırken seçenekleri temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | e-kitap dosyasını yüklemek için bir seçenek oluşturur. |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | e-kitap dosyasını yüklemek için bir seçenek oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Ekli dosyaların kaydedileceği dizin. |
| [getAutoFilter()](#getAutoFilter--) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Sütun ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Otomatik sığdırma seçeneklerini alır |
| [getCheckDataValid()](#getCheckDataValid--) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getConvertFormulasData()](#getConvertFormulasData--) | true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur. |
| [getConvertNumericData()](#getConvertNumericData--) | Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Metin, `<br>` etiketi kullanılarak satırları sararken gereksiz boşlukların silinip silinmeyeceğini gösterir. |
| [getDetectLaTeX()](#getDetectLaTeX--) | HTML dosyasında LaTeX formülünün tespit edilip edilmediğini gösterir. |
| [getEncoding()](#getEncoding--) | Varsayılan kodlamayı alır. |
| [getFontConfigs()](#getFontConfigs--) | Bireysel yazı tipi yapılandırmalarını alır. |
| [getHyperlinkLoadMode()](#getHyperlinkLoadMode--) | HTML yüklenirken köprülerin nasıl yükleneceğini belirtir. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Kesinti izleyicisini alır. |
| [getKeepPrecision()](#getKeepPrecision--) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [getLanguageCode()](#getLanguageCode--) | Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [getLoadFilter()](#getLoadFilter--) | Verinin nasıl yükleneceğini belirten filtre. |
| [getLoadFormat()](#getLoadFormat--) | Yükleme biçimini alır. |
| [getLoadFormulas()](#getLoadFormulas--) | Orijinal HTML dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir. |
| [getLocale()](#getLocale--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getMemorySetting()](#getMemorySetting--) | Yüklenen çalışma kitabı için bellek modunu alır. |
| [getParagrahLayoutMode()](#getParagrahLayoutMode--) | HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. |
| [getParagraphLayoutMode()](#getParagraphLayoutMode--) | HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getPassword()](#getPassword--) | Çalışma kitabının şifresini alır. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [getProgId()](#getProgId--) | Dosyayı oluşturan program kimliğini alır. |
| [getRegion()](#getRegion--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getStandardFont()](#getStandardFont--) | Varsayılan standart yazı tipi adını ayarlar |
| [getStandardFontSize()](#getStandardFontSize--) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [getStreamProvider()](#getStreamProvider--) | Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı alır. |
| [getSupportDivTag()](#getSupportDivTag--) | `<div>` etiketinin düzenini, HTML dosyası içerdiğinde destekleyip desteklemeyeceğini gösterir. |
| [getTableLoadOptions()](#getTableLoadOptions--) | HtmlTableLoadOptionCollection örneğini al. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hasFormula()](#hasFormula--) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Ekli dosyaların kaydedileceği dizin. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | Sütun ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Otomatik sığdırma seçeneklerini ayarlar |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | Metin, `<br>` etiketi kullanılarak satırları sararken gereksiz boşlukların silinip silinmeyeceğini gösterir. |
| [setDetectLaTeX(boolean value)](#setDetectLaTeX-boolean-) | HTML dosyasında LaTeX formülünün tespit edilip edilmediğini gösterir. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Varsayılan kodlamayı ayarlar. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Bireysel yazı tipi yapılandırmalarını ayarlar. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [setHyperlinkLoadMode(int value)](#setHyperlinkLoadMode-int-) | HTML yüklenirken köprülerin nasıl yükleneceğini belirtir. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Kesinti izleyicisini ayarlar. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Verinin nasıl yükleneceğini belirten filtre. |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | Orijinal HTML dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Yüklenen workbook için bellek modunu ayarlar. |
| [setPaperSize(int type)](#setPaperSize-int-) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. |
| [setParagrahLayoutMode(int value)](#setParagrahLayoutMode-int-) | HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. |
| [setParagraphLayoutMode(int value)](#setParagraphLayoutMode-int-) | HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Workbook'un şifresini ayarlar. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [setRegion(int value)](#setRegion-int-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Varsayılan standart yazı tipi adını ayarlar |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı ayarlar. |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | `<div>` etiketinin düzenini, HTML dosyası içerdiğinde destekleyip desteklemeyeceğini gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


e-kitap dosyasını yüklemek için bir seçenek oluşturur.

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


e-kitap dosyasını yüklemek için bir seçenek oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Yükleme biçimi |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Ekli dosyaların kaydedileceği dizin.

**Remarks**

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.StreamProvider özelliğini kullanın. Bu özellik Aralık 2014'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir.

**Remarks**

Bazen otomatik filtre ayarlı olsa da ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışır.

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


Sütun ve satırların otomatik olarak sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Otomatik sığdırma seçeneklerini alır

**Remarks**

Şu anda yalnızca xlsx, spreadsheetML dosyası için.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değeri alır. Varsayılan değer true'tur.

**Returns:**
boolean
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.HasFormula özelliğini kullanın. Bu özellik Mart 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değeri alır. Varsayılan değer true'tur.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


`<br>` etiketi kullanılarak metin satırları sarıldığında gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDetectLaTeX() {#getDetectLaTeX--}
```
public boolean getDetectLaTeX()
```


HTML dosyasında LaTeX formülünün algılanıp algılanmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Varsayılan kodlamayı alır. Yalnızca csv dosyası için geçerlidir.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Bireysel yazı tipi yapılandırmalarını alır. Yalnızca [Workbook](../../com.aspose.cells/workbook) bu [LoadOptions](../../com.aspose.cells/loadoptions) kullanılarak yüklendiğinde çalışır.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHyperlinkLoadMode() {#getHyperlinkLoadMode--}
```
public int getHyperlinkLoadMode()
```


HTML yüklenirken köprülerin nasıl yükleneceğini belirtir.

Bakınız [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar

**Remarks**

Yalnızca xlsx dosyası için.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir.

**Remarks**

Yalnızca xlsx, xlsb ve xlsm dosyaları için çalışır. Bazı dosyalarda işe yaramayan birçok üst üste binen aynı şekil vardır, dosyaları yüklerken bunları yok sayabiliriz.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Kesinti izleyicisini alır.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağı. Varsayılan değer true'tur.

**Remarks**

Kullanıcının yalnızca şablon dosyasından bazı içerikleri okuması ve workbook'u geri kaydetmeye ihtiyacı olmadığı senaryolarda, bu özelliği false olarak ayarlamak performansı artırabilir, özellikle bir tür LoadFilter ile birlikte kullanıldığında.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Verinin nasıl yükleneceğini belirten filtre.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Yükleme biçimini alır.

Bakınız [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


Orijinal HTML dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir.

**Returns:**
boolean
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir.

Bakınız [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır.

**Remarks**

Bu özellik, bölgesel ayarları belirlemek için [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) ile aynı etkiye sahiptir.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Yüklenen çalışma kitabı için bellek modunu alır.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bellek modu hakkında daha fazla ayrıntı için lütfen [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--) adresine bakın.

**Returns:**
int
### getParagrahLayoutMode() {#getParagrahLayoutMode--}
```
public int getParagrahLayoutMode()
```


HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. Varsayılan değer [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)dır.

Bakınız [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.ParagraphLayoutMode özelliğini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getParagraphLayoutMode() {#getParagraphLayoutMode--}
```
public int getParagraphLayoutMode()
```


HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. Varsayılan değer [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)dır.

Bakınız [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm ve Xlsm dosyalarına uygulanır çünkü dosyalardaki formüller dize formülü olarak depolanır.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm, Xlsm ve xlsb dosyalarına uygulanır.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Çalışma kitabının şifresini alır.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) bu özellik ile aynı değere ayarlanacaktır.

**Returns:**
boolean
### getProgId() {#getProgId--}
```
public String getProgId()
```


Dosyanın oluşturulması için program kimliğini alır. Yalnızca MHT dosyaları için.

**Returns:**
java.lang.String
### getRegion() {#getRegion--}
```
public int getRegion()
```


Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Bölgesel ayarlar, çalışma kitabı için yazı tipleri, temalar vb. gibi bazı özelliklerin başlatılmasında kullanılabilir. CSV, HTML gibi metin tabanlı dosya formatları için bölgesel ayar, sayı biçimlerini algılamak ve hücrelerdeki metin değerlerini sayısal veya tarih‑zaman değerlerine dönüştürmek için de kullanılacaktır. Bu ayar daha sonra oluşturulan çalışma kitabı için korunur; yani, çalışma kitabının [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) aynı bölgeyi bu özellik ile kullanacaktır.

**Returns:**
int
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Varsayılan standart yazı tipi adını ayarlar

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Varsayılan standart yazı tipi boyutunu ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
double
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı alır.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


HTML dosyası `<div>` etiketini içerdiğinde bu etiketin düzenini destekleyip desteklemediğini gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


HtmlTableLoadOptionCollection örneğini al.

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Uyarı geri çağrısını alır.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Ekli dosyaların kaydedileceği dizin.

**Remarks**

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.StreamProvider özelliğini kullanın. Bu özellik Aralık 2014'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir.

**Remarks**

Bazen otomatik filtre ayarlı olsa da ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


Sütun ve satırların otomatik olarak sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Otomatik sığdırma seçeneklerini ayarlar

**Remarks**

Şu anda yalnızca xlsx, spreadsheetML dosyası için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.HasFormula özelliğini kullanın. Bu özellik Mart 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


`<br>` etiketi kullanılarak metin satırları sarıldığında gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDetectLaTeX(boolean value) {#setDetectLaTeX-boolean-}
```
public void setDetectLaTeX(boolean value)
```


HTML dosyasında LaTeX formülünün algılanıp algılanmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Varsayılan kodlamayı ayarlar. Yalnızca csv dosyaları için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Bireysel yazı tipi yapılandırmalarını ayarlar. Yalnızca bu [LoadOptions](../../com.aspose.cells/loadoptions) ile yüklenen [Workbook](../../com.aspose.cells/workbook) için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHyperlinkLoadMode(int value) {#setHyperlinkLoadMode-int-}
```
public void setHyperlinkLoadMode(int value)
```


HTML yüklenirken köprülerin nasıl yükleneceğini belirtir.

Bakınız [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar

**Remarks**

Yalnızca xlsx dosyası için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir.

**Remarks**

Yalnızca xlsx, xlsb ve xlsm dosyaları için çalışır. Bazı dosyalarda işe yaramayan birçok üst üste binen aynı şekil vardır, dosyaları yüklerken bunları yok sayabiliriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Kesinti izleyicisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağı. Varsayılan değer true'tur.

**Remarks**

Kullanıcının yalnızca şablon dosyasından bazı içerikleri okuması ve workbook'u geri kaydetmeye ihtiyacı olmadığı senaryolarda, bu özelliği false olarak ayarlamak performansı artırabilir, özellikle bir tür LoadFilter ile birlikte kullanıldığında.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Verinin nasıl yükleneceğini belirten filtre.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


Orijinal HTML dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir.

Bakınız [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar.

**Remarks**

Bu özellik, bölgesel ayarları belirlemek için [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) ile aynı etkiye sahiptir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Yüklenen workbook için bellek modunu ayarlar.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bellek modu hakkında daha fazla ayrıntı için lütfen [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--) adresine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar.

**Remarks**

Kağıt boyutu ile ilgili bir ayar yoksa, MS Excel varsayılan yazıcı ayarını kullanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). Varsayılan kağıt boyutu. |

### setParagrahLayoutMode(int value) {#setParagrahLayoutMode-int-}
```
public void setParagrahLayoutMode(int value)
```


HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. Varsayılan değer [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)dır.

Bakınız [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.ParagraphLayoutMode özelliğini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setParagraphLayoutMode(int value) {#setParagraphLayoutMode-int-}
```
public void setParagraphLayoutMode(int value)
```


HTML yüklenirken HTML <p> öğelerinin nasıl işlendiğini belirtir. Varsayılan değer [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)dır.

Bakınız [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm ve Xlsm dosyalarına uygulanır çünkü dosyalardaki formüller dize formülü olarak depolanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm, Xlsm ve xlsb dosyalarına uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Workbook'un şifresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) bu özellik ile aynı değere ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Bölgesel ayarlar, çalışma kitabı için yazı tipleri, temalar vb. gibi bazı özelliklerin başlatılmasında kullanılabilir. CSV, HTML gibi metin tabanlı dosya formatları için bölgesel ayar, sayı biçimlerini algılamak ve hücrelerdeki metin değerlerini sayısal veya tarih‑zaman değerlerine dönüştürmek için de kullanılacaktır. Bu ayar daha sonra oluşturulan çalışma kitabı için korunur; yani, çalışma kitabının [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) aynı bölgeyi bu özellik ile kullanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Varsayılan standart yazı tipi adını ayarlar

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Varsayılan standart yazı tipi boyutunu ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


HTML dosyası `<div>` etiketini içerdiğinde bu etiketin düzenini destekleyip desteklemediğini gösterir. Varsayılan değer false'tur.

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

