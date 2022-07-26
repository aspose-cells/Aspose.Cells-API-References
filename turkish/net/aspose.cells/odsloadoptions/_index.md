---
title: OdsLoadOptions
second_title: Aspose.Cells for .NET API Referansı
description: ods dosyasını yükleme seçeneklerini temsil eder.
type: docs
weight: 4330
url: /tr/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

ods dosyasını yükleme seçeneklerini temsil eder.

```csharp
public class OdsLoadOptions : LoadOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [OdsLoadOptions](odsloadoptions#constructor)() | ods dosyasını yükleme seçeneklerini temsil eder. |
| [OdsLoadOptions](odsloadoptions#constructor_1)(LoadFormat) | ods dosyasını yükleme seçeneklerini temsil eder. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink) { get; set; } | Excel'in varsayılan stilinin köprüye uygulanıp uygulanmayacağını gösterir. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Dosyaları yüklerken verilerin otomatik olarak filtrelenip filtrelenmediğini gösterir. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Otomatik montaj seçeneklerini alır ve ayarlar |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol edin. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasını kontrol edip etmediğini kontrol edin. Örneğin, excel 32K'dan daha uzun dize değerlerinin girilmesine izin vermez. Cell.PutValue(dize) gibi 32K'dan daha uzun bir değer girdiğinizde, eğer bu özellik true ise, bir İstisna alırsınız. Bu özellik false ise, girdi dizesi değerinizi hücrenin değeri olarak kabul ederiz, böylece later , CSV. gibi diğer dosya biçimleri için tam dize değerini yazdırabilirsiniz. excel dosya formatı için geçersiz bir değer belirlediniz, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen bir hata oluşabilir. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Dosyanın yüklendiği andaki sistem kültürü bilgisini alır veya ayarlar. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Ayrı yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca şunlar için çalışır:[`Workbook`](../workbook) bunu kullanan[`LoadOptions`](../loadoptions) yüklemek için.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Dosyayı doğrudan yazdırıyorsanız yazdırılmayan verileri yoksayın |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Kesinti izleyicisini alır ve ayarlar. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Şablon dosyasından yüklendiğinde Çalışma Kitabı için çözümlenmemiş verilerin bellekte tutulup tutulmayacağı. Varsayılan true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Dosyayı kaydeden Ülke Koduna göre Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Şablon dosyasını okurken hücre verilerini işlemek için veri işleyici. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Verilerin nasıl yükleneceğini gösteren filtre. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Yükleme biçimini alır. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Bellek kullanım seçeneklerini alır veya ayarlar. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Dosya yüklenirken pivot önbelleğe alınmış kayıtların ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Çalışma kitabının parolasını alır ve ayarlar. |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables) { get; set; } | Dosya yüklenirken pivot tabloların yenilenip yenilenmediğini gösterir. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Dosyanın yüklendiği andaki Ülke Koduna göre sistem bölgesel ayarlarını alır veya ayarlar. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Varsayılan yazıcı ayarından varsayılan yazdırma kağıdı boyutunu ayarlar. |

### Ayrıca bakınız

* class [LoadOptions](../loadoptions)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
