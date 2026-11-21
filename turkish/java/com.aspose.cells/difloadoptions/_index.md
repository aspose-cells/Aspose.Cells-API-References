---
title: "DifLoadOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: ".dif dosyasını yükleme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/difloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class DifLoadOptions extends LoadOptions
```

.dif dosyasını yükleme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DifLoadOptions()](#DifLoadOptions--) | Seçenekler. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Otomatik sığdırma seçeneklerini alır |
| [getCheckDataValid()](#getCheckDataValid--) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [getFontConfigs()](#getFontConfigs--) | Bireysel yazı tipi yapılandırmalarını alır. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Kesinti izleyicisini alır. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [getLanguageCode()](#getLanguageCode--) | Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [getLoadFilter()](#getLoadFilter--) | Verinin nasıl yükleneceğini belirten filtre. |
| [getLoadFormat()](#getLoadFormat--) | Yükleme biçimini alır. |
| [getLocale()](#getLocale--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getMemorySetting()](#getMemorySetting--) | Yüklenen çalışma kitabı için bellek modunu alır. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getPassword()](#getPassword--) | Çalışma kitabının şifresini alır. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [getRegion()](#getRegion--) | Yüklenecek Çalışma Kitabı için kullanılan bölgesel ayarları alır. |
| [getStandardFont()](#getStandardFont--) | Varsayılan standart yazı tipi adını ayarlar |
| [getStandardFontSize()](#getStandardFontSize--) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Otomatik sığdırma seçeneklerini ayarlar |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Bireysel yazı tipi yapılandırmalarını ayarlar. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gereksiz şekillerin yoksayılıp yoksayılmadığını gösterir. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Kesinti izleyicisini ayarlar. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Verinin nasıl yükleneceğini belirten filtre. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Yüklenen workbook için bellek modunu ayarlar. |
| [setPaperSize(int type)](#setPaperSize-int-) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Workbook'un şifresini ayarlar. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [setRegion(int value)](#setRegion-int-) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları ayarlar. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Varsayılan standart yazı tipi adını ayarlar |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Varsayılan standart yazı tipi boyutunu ayarlar. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DifLoadOptions() {#DifLoadOptions--}
```
public DifLoadOptions()
```


Seçenekler.

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
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Bireysel yazı tipi yapılandırmalarını alır. Yalnızca [Workbook](../../com.aspose.cells/workbook) bu [LoadOptions](../../com.aspose.cells/loadoptions) kullanılarak yüklendiğinde çalışır.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
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

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Bireysel yazı tipi yapılandırmalarını ayarlar. Yalnızca bu [LoadOptions](../../com.aspose.cells/loadoptions) ile yüklenen [Workbook](../../com.aspose.cells/workbook) için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

