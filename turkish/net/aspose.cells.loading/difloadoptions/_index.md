---
title: "Sınıf DifLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Loading.DifLoadOptions sınıfı. .dif dosyasını yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Bir .dif dosyasını yükleme seçeneklerini temsil eder.

```csharp
public class DifLoadOptions : LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Seçenekler. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir. ([`LoadOptions`](../../aspose.cells/loadoptions/) üzerinden devralınmıştır.) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Otomatik sığdırıcı seçeneklerini alır ve ayarlar ([`LoadOptions`](../../aspose.cells/loadoptions/) üzerinden devralınmıştır.) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını denetler. ([`LoadOptions`](../../aspose.cells/loadoptions/) üzerinden devralınmıştır.) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. ([`LoadOptions`](../../aspose.cells/loadoptions/) üzerinden devralınmıştır.) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Yüklenmekte olan Çalışma Kitabı için kullanılan bölgesel ayarları alır veya ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca bu [`LoadOptions`](../../aspose.cells/loadoptions/) ile yükleyen [`Workbook`](../../aspose.cells/workbook/) için çalışır.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gereksiz şekillerin yoksayılıp yoksayılmayacağını gösterir.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirler. Varsayılan değer doğrudur.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode'a göre Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır veya ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Verilerin nasıl yükleneceğini belirtmek için filtre.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Yükleme formatını alır.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Yüklenen çalışma kitabı için bellek modunu alır veya ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer yanlıştır.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Çalışma kitabının şifresini alır ve ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Formülleri alırken ve ayarlarken formül belirteçleri arasında eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer yanlıştır.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Yüklenmekte olan Çalışma Kitabı için kullanılan bölgesel ayarları alır veya ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi adını ayarlar(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi boyutunu ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar.(Miras alınan [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // DifLoadOptions örneği oluştur
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Parametresiz yapıcı kullanarak bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Varsa formülleri hesaplayın
            workbook.CalculateFormula();

            // Çalışma kitabını DIF formatında kaydedin
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Şimdi DifLoadOptions ile DIF dosyasını yüklemeyi gösterin
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Kaydedilen DIF dosyasını seçeneklerle yükleyin
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Yüklenen çalışma kitabından verilere erişin
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Yüklenen verileri doğrulama için XLSX olarak kaydedin
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


