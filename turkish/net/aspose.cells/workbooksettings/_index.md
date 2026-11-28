---
title: "WorkbookSettings sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WorkbookSettings sınıfı. Çalışma kitabının tüm ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Çalışma kitabının tüm ayarlarını temsil eder.

```csharp
public class WorkbookSettings : IDisposable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Dosyanın yazarını alır ve ayarlar. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirtir. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Uygulamanın artımlı genel sürümünü belirtir. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Sistem kültür bilgilerini alır veya ayarlar. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Görselin varsayılan çözünürlüğünü alır ve ayarlar. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Görsel düzenleme verilerinin atılıp atılmadığını gösterir. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Çalışma kitabındaki nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini gösterir. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Makroları etkinleştir; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | İlk görünen çalışma sayfası sekmesini alır veya ayarlar. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Formül ile ilgili özelliklerin ayarlarını alır. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Küreselleştirme ayarlarını alır ve ayarlar. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | PivotTable için alan listesinin gizlenip gizlenmeyeceğini alır ve ayarlar. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Çalışma kitabının Yapısı ve Pencereleri kilitli ise varsayılan şifreyle şifrelenip şifrelenmediğini gösterir. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Bu çalışma kitabını açmak için bir şifre gerekip gerekmediğini gösteren bir değeri alır. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Çalışma kitabının yapısının veya penceresinin korunup korunmadığını gösteren bir değeri alır. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini belirten bir değeri alır veya ayarlar. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode temelinde Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Sıfır tabanlı maksimum sütun dizinini alır. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Sıfır tabanlı maksimum satır dizinini alır. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Paylaşılan formülün maksimum satır sayısını alır ve ayarlar. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Alan başına benzersiz öğe sınırlamasını alır ve ayarlar. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Bellek kullanımı seçeneklerini alır veya ayarlar. Yeni seçenek, yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınır ancak mevcut çalışma sayfaları için etkili olmaz. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Sayısal değerlerde ondalık noktasının solundaki rakam gruplarını ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcıdır. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Varsayılan yazdırma kağıt boyutunu alır ve ayarlar. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Workbook dosya şifreleme parolasını temsil eder. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Workbook'un koruma türünü alır. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Hücreye tek tırnak işaretiyle başlayan dize değeri girilirken [`QuotePrefix`](../style/quoteprefix/) özelliğinin ayarlanıp ayarlanmadığını gösterir. |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Workbook için bölgesel ayarları alır veya ayarlar. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Belirtilen çalışma kitabından kişisel bilgiler kaldırılabiliyorsa doğru döner. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Harici kaynak için akış sağlayıcısını alır ve ayarlar, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi. |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntülediğini alır ve ayarlar. |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Workbook'un paylaşılıp paylaşılmadığını belirten bir değeri alır veya ayarlar. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Workbook sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Önemli basamak sayısını alır ve ayarlar. Varsayılan değer [`SignificantDigits`](../cellshelper/significantdigits/) dir. |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Bu çalışma kitabındaki sayısal değerlerin çıktısı için önemli basamak türünü alır ve ayarlar. Varsayılan değer [`SignificantDigitsType`](../cellshelper/significantdigitstype/) dir. |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Akıllı etiketin seçeneklerini alır. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Eski.**) Dış kaynak için akış sağlayıcısını alır ve ayarlar. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Komşu hücrelerin kenarlığını güncelleyip güncellemeyeceğini belirtir. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Çalışma kitabı açıldığında dış bağlantıların nasıl güncelleneceğini alır ve ayarlar. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | Pencerenin yüksekliği, nokta biriminde. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | Pencerenin yüksekliği, santimetre biriminde. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | Pencerenin yüksekliği, inç biriminde. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, santimetre biriminde. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, inç biriminde. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | Pencerenin genişliği, nokta biriminde. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | Pencerenin genişliği, santimetre biriminde. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | Pencerenin genişliği, inç biriminde. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | WPS ile uyumlu olup olmadığını gösterir. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Çalışma kitabının yazma koruma seçeneklerine erişim sağlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Kaynakları serbest bırakır. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Varsayılan tema yazı tipi adını alır. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Tüm çalışma kitabı için baskı yönlendirme tipini ayarlar. |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Yeni bir çalışma kitabı oluştur
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Örnek veri ekleyin
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // WorkbookSettings'a erişin.
        WorkbookSettings settings = workbook.Settings;

        // Çeşitli ayarları ayarlayın.
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Çalışma kitabını kaydedin
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


