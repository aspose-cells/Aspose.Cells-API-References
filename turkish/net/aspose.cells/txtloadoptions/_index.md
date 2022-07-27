---
title: TxtLoadOptions
second_title: Aspose.Cells for .NET API Referansı
description: Metin dosyası yükleme seçeneklerini temsil eder.
type: docs
weight: 6110
url: /tr/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Metin dosyası yükleme seçeneklerini temsil eder.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | Metin dosyası yükleme seçeneklerini oluşturur. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | Metin dosyası yükleme seçeneklerini oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Dosyaları yüklerken verilerin otomatik olarak filtrelenip filtrelenmediğini gösterir. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Otomatik montaj seçeneklerini alır ve ayarlar |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol edin. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasını kontrol edip etmediğini kontrol edin. Örneğin, excel 32K'dan daha uzun dize değerlerinin girilmesine izin vermez. Cell.PutValue(dize) gibi 32K'dan daha uzun bir değer girdiğinizde, eğer bu özellik true ise, bir İstisna alırsınız. Bu özellik false ise, girdi dizesi değerinizi hücrenin değeri olarak kabul ederiz, böylece later , CSV. gibi diğer dosya biçimleri için tam dize değerini yazdırabilirsiniz. excel dosya formatı için geçersiz bir değer belirlediniz, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen bir hata oluşabilir. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Metin dosyasındaki dizenin tarih verilerine dönüştürülüp dönüştürülmediğini gösteren bir değer alır veya ayarlar. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Metin dosyasındaki dizenin sayısal verilere dönüştürülüp dönüştürülmediğini gösteren bir değer alır veya ayarlar. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Dosyanın yüklendiği andaki sistem kültürü bilgisini alır veya ayarlar. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | Veri satırları veya sütunları limiti aştığında veriyi bir sonraki sayfaya genişletip genişletmeyeceği. Bu özellik doğruysa, mevcut sayfanın arkasındaki bir sonraki sayfaya ekstra veri genişletilir (eğer mevcut sayfa sonuncuysa, yeni sayfa eklenir geçerli çalışma kitabına). Bu özellik yanlışsa, sınırı aşan veriler yok sayılır. Varsayılan yanlıştır; |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Ayrı yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca şunlar için çalışır:[`Workbook`](../workbook) bunu kullanan[`LoadOptions`](../loadoptions) yüklemek için.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | Metnin "=" ile başlıyorsa formül olup olmadığını gösterir. |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | Hücre değeri için metin niteleyicisi olup olmadığı. Varsayılan true. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Dosyayı doğrudan yazdırıyorsanız yazdırılmayan verileri yoksayın |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Kesinti izleyicisini alır ve ayarlar. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | Doğru, dosyanın birkaç kodlama içerdiği anlamına gelir. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Uzunluk 15. ise bir dize değerinin ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Şablon dosyasından yüklendiğinde Çalışma Kitabı için çözümlenmemiş verilerin bellekte tutulup tutulmayacağı. Varsayılan true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Dosyayı kaydeden Ülke Koduna göre Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Şablon dosyasını okurken hücre verilerini işlemek için veri işleyici. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Verilerin nasıl yükleneceğini gösteren filtre. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Yükleme biçimini alır. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Dize değerini sayıya veya tarih saatine dönüştürürken ayrıştırılmış değerler için stil uygulama stratejisini belirtir. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Bellek kullanım seçeneklerini alır veya ayarlar. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Dosya yüklenirken pivot önbelleğe alınmış kayıtların ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Çalışma kitabının parolasını alır ve ayarlar. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | Metin dosyasını yüklemek için tercih edilen değer ayrıştırıcılarını alır ve ayarlar. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Dosyanın yüklendiği andaki Ülke Koduna göre sistem bölgesel ayarlarını alır veya ayarlar. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | Metin dosyasının karakter ayırıcısını alır ve ayarlar. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | Ayırıcı olarak bir dize değeri alır ve ayarlar. |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | Ardışık sınırlayıcıların tek olarak kabul edilip edilmeyeceği. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | Öndeki tek tırnak işaretinin bir hücrenin değerinin parçası olarak alınması gerekip gerekmediğini gösterir. Varsayılan doğrudur. Yanlışsa, baştaki tek tırnak ilgili hücrenin value değerinden kaldırılır ve[`QuotePrefix`](../style/quoteprefix) hücre için doğru olarak ayarlanacaktır. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Varsayılan yazıcı ayarından varsayılan yazdırma kağıdı boyutunu ayarlar. |

### Ayrıca bakınız

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
