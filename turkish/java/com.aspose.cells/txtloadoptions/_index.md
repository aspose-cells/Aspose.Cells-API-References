---
title: "TxtLoadOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Metin dosyası yükleme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Metin dosyası yükleme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Metin dosyasını yüklemek için seçenekleri oluşturur. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Metin dosyasını yüklemek için seçenekleri oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Otomatik sığdırma seçeneklerini alır |
| [getCheckDataValid()](#getCheckDataValid--) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getConvertNumericData()](#getConvertNumericData--) | Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [getEncoding()](#getEncoding--) | Varsayılan kodlamayı alır. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Veri satırları veya sütunları limit aşınca veriyi bir sonraki sayfaya genişletip genişletmeyeceğini belirler. |
| [getFontConfigs()](#getFontConfigs--) | Bireysel yazı tipi yapılandırmalarını alır. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | Genişletilmiş sayfalar için tekrarlanacak başlık satırlarının sayısı. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Kesinti izleyicisini alır. |
| [getKeepPrecision()](#getKeepPrecision--) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [getLanguageCode()](#getLanguageCode--) | Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [getLoadFilter()](#getLoadFilter--) | Verinin nasıl yükleneceğini belirten filtre. |
| [getLoadFormat()](#getLoadFormat--) | Yükleme biçimini alır. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir. |
| [getLocale()](#getLocale--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getMaxColumnCount()](#getMaxColumnCount--) | Bir sayfa için içe aktarılacak maksimum sütun sayısı. |
| [getMaxRowCount()](#getMaxRowCount--) | Bir sayfaya aktarılacak maksimum satır sayısı. |
| [getMemorySetting()](#getMemorySetting--) | Yüklenen çalışma kitabı için bellek modunu alır. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getPassword()](#getPassword--) | Çalışma kitabının şifresini alır. |
| [getPreferredParsers()](#getPreferredParsers--) | Metin dosyası yüklemek için tercih edilen değer ayrıştırıcılarını alır. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [getRegion()](#getRegion--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getSeparator()](#getSeparator--) | Metin dosyasının karakter ayırıcıyı alır. |
| [getSeparatorString()](#getSeparatorString--) | Ayırıcı olarak bir dize değeri alır. |
| [getStandardFont()](#getStandardFont--) | Varsayılan standart yazı tipi adını ayarlar |
| [getStandardFontSize()](#getStandardFontSize--) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [getTextQualifier()](#getTextQualifier--) | Hücre değerleri için metin niteleyicisini belirtir. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hasFormula()](#hasFormula--) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [hasTextQualifier()](#hasTextQualifier--) | Hücre değeri için metin niteleyicisinin olup olmadığı. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Otomatik sığdırma seçeneklerini ayarlar |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Varsayılan kodlamayı ayarlar. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Veri satırları veya sütunları limit aşınca veriyi bir sonraki sayfaya genişletip genişletmeyeceğini belirler. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Bireysel yazı tipi yapılandırmalarını ayarlar. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Hücre değeri için metin niteleyicisinin olup olmadığı. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | Genişletilmiş sayfalar için tekrarlanacak başlık satırlarının sayısı. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Kesinti izleyicisini ayarlar. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Verinin nasıl yükleneceğini belirten filtre. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini gösterir. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | Bir sayfa için içe aktarılacak maksimum sütun sayısı. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | Bir sayfaya aktarılacak maksimum satır sayısı. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Yüklenen workbook için bellek modunu ayarlar. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir. |
| [setPaperSize(int type)](#setPaperSize-int-) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Workbook'un şifresini ayarlar. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Metin dosyası yüklemek için tercih edilen değer ayrıştırıcılarını ayarlar. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [setRegion(int value)](#setRegion-int-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setSeparator(char value)](#setSeparator-char-) | Metin dosyasının karakter ayırıcıyı ayarlar. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Ayırıcı olarak bir dize değeri ayarlar. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Varsayılan standart yazı tipi adını ayarlar |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Hücre değerleri için metin niteleyicisini belirtir. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Metin dosyasını yüklemek için seçenekleri oluşturur.

**Remarks**

Varsayılan yükleme dosya türü CSV'dir.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Metin dosyasını yüklemek için seçenekleri oluşturur.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir.

**Remarks**

Bazen otomatik filtre ayarlı olsa da ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışır.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Varsayılan kodlamayı alır. Yalnızca csv dosyası için geçerlidir.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Veri satırları veya sütunları sınırı aştığında verinin bir sonraki sayfaya genişletilip genişletilmeyeceği. Varsayılan değer false.

**Remarks**

Bu özellik true ise, ekstra veri mevcut sayfanın arkasındaki bir sonraki sayfaya konulacaktır (eğer mevcut sayfa son sayfa ise, yeni sayfa mevcut çalışma kitabına eklenecektir). Bu özellik false ise, sınırı aşan veri yok sayılacaktır.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Bireysel yazı tipi yapılandırmalarını alır. Yalnızca [Workbook](../../com.aspose.cells/workbook) bu [LoadOptions](../../com.aspose.cells/loadoptions) kullanılarak yüklendiğinde çalışır.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı.

**Remarks**

Bu özellik tarafından belirtilen başlık sütunları, genişletilen sayfalar için çoğaltılacaktır. Bu özellik yalnızca [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) true olduğunda etkili olur.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


Genişletilmiş sayfalar için tekrarlanacak başlık satırlarının sayısı.

**Remarks**

Bu özellik tarafından belirtilen başlık satırları, genişletilen sayfalar için çoğaltılacaktır. Bu özellik yalnızca [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) true olduğunda etkili olur.

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
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


Bir sayfa için içe aktarılacak maksimum sütun sayısı.

**Remarks**

Bu sınırı aşan sütunlar, [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--)'a göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık sütunlarını ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)) içerir. Bunun maksimum değeri, ilgili dosya formatının sütun sınırıdır; örneğin xlsx dosyası için 16384'tür. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, maksimum sınır da kullanılacaktır.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


Bir sayfaya aktarılacak maksimum satır sayısı.

**Remarks**

Bu sınırı aşan satırlar, [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--)'a göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık satırlarını ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)) içerir. Bunun izin verilen maksimum değeri, ilgili dosya formatının satır sınırıdır; örneğin xlsx dosyası için 1048576'tır. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, maksimum sınır da kullanılacaktır.

**Returns:**
int
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
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Metin dosyası yüklemek için tercih edilen değer ayrıştırıcılarını alır.

**Remarks**

parsers[0] metin şablon dosyasındaki ilk sütun için kullanılacak ayrıştırıcıdır, parsers[1] ikinci sütun için kullanılacak ayrıştırıcıdır, ... vb. Sonuncusu (parsers[parsers.length-1]) parsers.length-1'den başlayan tüm diğer sütunlar için kullanılacaktır. Bir öğe null ise, ilgili sütun Aspose.Cells'in varsayılan ayrıştırıcısı tarafından ayrıştırılacaktır.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) bu özellik ile aynı değere ayarlanacaktır.

**Returns:**
boolean
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Metin dosyasının karakter ayırıcıyı alır.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ayırıcı olarak bir dize değeri alır.

**Returns:**
java.lang.String
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
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '"'dir.

**Remarks**

Bu özellik ayarlandığında, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) otomatik olarak true olacaktır.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. Varsayılan değer true'tır. False ise, başlangıçtaki tek tırnak ilgili hücrenin değerinden kaldırılacak ve [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) hücre için true olarak ayarlanacaktır.

**Returns:**
boolean
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
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir.

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

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. Varsayılan değer true'tur.

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

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Veri satırları veya sütunları sınırı aştığında verinin bir sonraki sayfaya genişletilip genişletilmeyeceği. Varsayılan değer false.

**Remarks**

Bu özellik true ise, ekstra veri mevcut sayfanın arkasındaki bir sonraki sayfaya konulacaktır (eğer mevcut sayfa son sayfa ise, yeni sayfa mevcut çalışma kitabına eklenecektir). Bu özellik false ise, sınırı aşan veri yok sayılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı.

**Remarks**

Bu özellik tarafından belirtilen başlık sütunları, genişletilen sayfalar için çoğaltılacaktır. Bu özellik yalnızca [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) true olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


Genişletilmiş sayfalar için tekrarlanacak başlık satırlarının sayısı.

**Remarks**

Bu özellik tarafından belirtilen başlık satırları, genişletilen sayfalar için çoğaltılacaktır. Bu özellik yalnızca [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) true olduğunda etkili olur.

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

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


Bir sayfa için içe aktarılacak maksimum sütun sayısı.

**Remarks**

Bu sınırı aşan sütunlar, [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--)'a göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık sütunlarını ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)) içerir. Bunun maksimum değeri, ilgili dosya formatının sütun sınırıdır; örneğin xlsx dosyası için 16384'tür. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, maksimum sınır da kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


Bir sayfaya aktarılacak maksimum satır sayısı.

**Remarks**

Bu sınırı aşan satırlar, [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--)'a göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık satırlarını ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)) içerir. Bunun izin verilen maksimum değeri, ilgili dosya formatının satır sınırıdır; örneğin xlsx dosyası için 1048576'tır. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, maksimum sınır da kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Metin dosyası yüklemek için tercih edilen değer ayrıştırıcılarını ayarlar.

**Remarks**

parsers[0] metin şablon dosyasındaki ilk sütun için kullanılacak ayrıştırıcıdır, parsers[1] ikinci sütun için kullanılacak ayrıştırıcıdır, ... vb. Sonuncusu (parsers[parsers.length-1]) parsers.length-1'den başlayan tüm diğer sütunlar için kullanılacaktır. Bir öğe null ise, ilgili sütun Aspose.Cells'in varsayılan ayrıştırıcısı tarafından ayrıştırılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Metin dosyasının karakter ayırıcıyı ayarlar.

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

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '"'dir.

**Remarks**

Bu özellik ayarlandığında, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) otomatik olarak true olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. Varsayılan değer true'tır. False ise, başlangıçtaki tek tırnak ilgili hücrenin değerinden kaldırılacak ve [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) hücre için true olarak ayarlanacaktır.

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

