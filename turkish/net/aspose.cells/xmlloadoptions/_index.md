---
title: "Class XmlLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.XmlLoadOptions class. XML yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/
---
## XmlLoadOptions class

Xml yükleme seçeneklerini temsil eder.

```csharp
public class XmlLoadOptions : LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [XmlLoadOptions](xmlloadoptions/#constructor)() | XML dosyası yükleme seçeneklerini temsil eder |
| [XmlLoadOptions](xmlloadoptions/#constructor_1)(LoadFormat) | XML dosyası yükleme seçeneklerini temsil eder |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Otomatik sığdırma seçeneklerini alır ve ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ContainsMultipleWorksheets](../../aspose.cells/xmlloadoptions/containsmultipleworksheets/) { get; set; } | XML'in birden çok çalışma sayfası olarak içe aktarılıp aktarılmadığını gösterir. |
| [ConvertNumericOrDate](../../aspose.cells/xmlloadoptions/convertnumericordate/) { get; set; } | XML dosyasındaki değerin sayısal veya tarih formatına dönüştürülüp dönüştürülmediğini gösterir. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DateFormat](../../aspose.cells/xmlloadoptions/dateformat/) { get; set; } | Tarih değerinin biçimini alır ve ayarlar. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | workbook için stil başlatma varsayılan ayarlarını alır(Inherited from [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Bireysel font yapılandırmalarını alır ve ayarlar. Bu [`LoadOptions`](../loadoptions/) ile yüklenen [`Workbook`](../workbook/) için yalnızca çalışır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken basılmayan verileri yoksayar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreRootAttributes](../../aspose.cells/xmlloadoptions/ignorerootattributes/) { get; set; } | Kök öğenin özniteliklerini yoksayıp yoksamama durumunu gösterir. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Kullanışsız şekillerin yoksayılıp yoksayılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsXmlMap](../../aspose.cells/xmlloadoptions/isxmlmap/) { get; set; } | XML'nin Excel'e eşlenip eşlenmediğini gösterir. Varsayılan değer false'tur. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Workbook için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirtir. Varsayılan true'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode'a dayalı olarak Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Verilerin nasıl yükleneceğini belirten filtre.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Yükleme biçimini alır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Yüklenen workbook için bellek modunu alır veya ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [NumberFormat](../../aspose.cells/xmlloadoptions/numberformat/) { get; set; } | Sayısal değerin biçimini alır ve ayarlar. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Workbook'un şifresini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Formülleri alırken ve ayarlarken formül belirteçleri arasına eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. (Miras alınan [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi adını ayarlar(Miras alınan [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi boyutunu ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |
| [StartCell](../../aspose.cells/xmlloadoptions/startcell/) { get; set; } | Başlangıç hücresini alır ve ayarlar. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsDemo
    {
        public static void XmlLoadOptionsExample()
        {
            // XmlLoadOptions sınıfının bir örneğini oluştur.
            XmlLoadOptions options = new XmlLoadOptions();

            // Özellikleri ayarlama
            options.StartCell = "A1";
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = "0.00";
            options.DateFormat = "yyyy-MM-dd";
            options.IgnoreRootAttributes = false;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            options.LightCellsDataHandler = null; // Assuming no data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = null; // Assuming no individual font configs are set
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = false;

            // Belirtilen seçenekleri kullanarak bir XML dosyasını Çalışma Kitabı'na yükle.
            Workbook workbook = new Workbook("XmlLoadOptionsExample_original.xml", options);
            workbook.DefaultStyle.Font.Name = "Arial";  
            workbook.DefaultStyle.Font.Size = 10;
            
            // Çalışma kitabını yeni bir dosyaya kaydet
            workbook.Save("XmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


