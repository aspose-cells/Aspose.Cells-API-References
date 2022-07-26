---
title: WorkbookSettings
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabının tüm ayarlarını temsil eder.
type: docs
weight: 6500
url: /tr/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Çalışma kitabının tüm ayarlarını temsil eder.

```csharp
public class WorkbookSettings : IDisposable
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Dosyanın yazarını alır ve ayarlar. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını belirten bir boole değeri belirtir. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Uygulamanın artımlı genel sürümünü belirtir. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Çalışma kitabını kaydederken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Style.Custom. ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini gösterir. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasını kontrol edip etmediğini kontrol edin. Örneğin, excel 32K'dan daha uzun dize değerlerinin girilmesine izin vermez. Cell.PutValue(dize) gibi 32K'dan daha uzun bir değer girdiğinizde, eğer bu özellik true ise, bir İstisna alırsınız. Bu özellik false ise, girdi dizesi değerinizi hücrenin değeri olarak kabul ederiz, böylece later , CSV. gibi diğer dosya biçimleri için tam dize değerini yazdırabilirsiniz. excel dosya formatı için geçersiz bir değer belirlediniz, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen bir hata oluşabilir. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | , uygulamanın bir kilitlenmeden sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Sistem kültürü bilgisini alır veya ayarlar. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | , uygulamanın çalışma kitabını veri kurtarma için en son açıp açmadığını gösterir. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını gösteren bir değer alır veya ayarlar. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Çalışma kitabındaki nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Makroları etkinleştir; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | İlk görünür çalışma sayfası sekmesini alır veya ayarlar. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Formülle ilgili özelliklerin ayarlarını alır. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Küreselleştirme ayarlarını alır ve ayarlar. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | PivotTable için alan listesinin gizlenip gizlenmeyeceğini ayarlar. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Çalışma kitabının Yapısı ve Pencereleri kilitliyse, çalışma kitabının varsayılan parolayla şifrelenip şifrelenmediğini gösterir. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Bu çalışma kitabını açmak için parola gerekip gerekmediğini belirten bir değer alır. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermediğini belirten bir değer alır veya ayarlar. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Çalışma Kitabının yapısının mı yoksa penceresinin mi korunduğunu gösteren bir değer alır. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermediğini belirten bir değer alır veya ayarlar. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Dosyayı kaydeden Ülke Koduna göre Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Sıfır tabanlı maksimum sütun dizinini alır. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Sıfır tabanlı maksimum satır dizinini alır. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Paylaşılan formülün maksimum satır sayısını alır ve ayarlar. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Bellek kullanım seçeneklerini alır veya ayarlar. Yeni seçenek, yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınacaktır ancak mevcut çalışma sayfaları için geçerli olmayacaktır. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Sayısal değerleri biçimlendirme/ayrıştırma için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Ondalık sayının solundaki basamak gruplarını sayısal değerlerle ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcısıdır. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Varsayılan baskı kağıdı boyutunu alır ve ayarlar. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Çalışma Kitabı dosya şifreleme parolasını temsil eder. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Çalışma kitabının koruma türünü alır. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Ayarın yapılıp yapılmayacağını gösterir.[`QuotePrefix`](../style/quoteprefix) hücresine dize değeri (tek tırnak işaretiyle başlayan) girerken özellik |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Çalışma kitabı için bölgesel ayarları alır veya ayarlar. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | Kişisel bilgiler belirtilen çalışma kitabından kaldırılabiliyorsa doğrudur. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Uygulamanın çalışma kitabını en son güvenli modda mı yoksa onarım modunda mı açtığını gösterir. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | "LinkToFile" türündeki resim için görüntü verilerinin yüklenmesi gibi harici kaynak için akış sağlayıcısını alır ve ayarlar. |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Çalışma Kitabının paylaşılıp paylaşılmadığını gösteren bir değer alır veya ayarlar. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'inde). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Çalışma Kitabı sekmelerinin görüntülenip görüntülenmeyeceği konusunda bir değer alır veya ayarlar. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Önemli basamakların sayısını alır ve ayarlar. Varsayılan değer[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Bitişik hücrelerin kenarlığının güncellenip güncellenmediğini gösterir. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Çalışma kitabı açıldığında harici bağlantıların nasıl güncelleneceğini alır ve ayarlar. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | Nokta birimi cinsinden pencerenin yüksekliği. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | Santimetre cinsinden pencerenin yüksekliği. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | Pencerenin inç cinsinden yüksekliği. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına kadar olan mesafe, nokta birimi olarak. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına kadar olan mesafe. Santimetre birimi olarak. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına kadar olan mesafe. İnç birimi olarak. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına kadar olan mesafe, nokta birimi olarak. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına kadar olan mesafe, santimetre biriminde. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına kadar olan mesafe, inç biriminde. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | Nokta birimi cinsinden pencerenin genişliği. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | Santimetre cinsinden pencerenin genişliği. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | Pencerenin inç cinsinden genişliği. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Çalışma kitabı yazma koruması seçeneklerine erişim sağlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Kaynakları serbest bırakır. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Varsayılan tema yazı tipi adını alır. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Tüm çalışma kitabı için yazdırma yönü türünü ayarlayın. |

### Örnekler

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//işini yap

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'işini yap
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
