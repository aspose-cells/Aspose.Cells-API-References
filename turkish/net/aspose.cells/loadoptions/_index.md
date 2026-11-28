---
title: "Sınıf LoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LoadOptions sınıfı. Dosyanın yüklenme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/loadoptions/
---
## LoadOptions class

Dosyayı yükleme seçeneklerini temsil eder.

```csharp
public class LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Dosyayı yükleme seçeneklerini oluşturur. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Dosyayı yükleme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Otomatik sığdırma seçeneklerini alır ve ayarlar |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol et. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca bu `LoadOptions`ı kullanarak yükleyen [`Workbook`](../workbook/) için çalışır. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yok say. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gereksiz şekillerin yok sayılıp sayılmayacağını gösterir. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Çalışma kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirler. Varsayılan değer doğrudur. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode temelinde Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Verilerin nasıl yükleneceğini belirten filtre. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Yükleme biçimini alır. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Yüklenen çalışma kitabı için bellek modunu alır veya ayarlar. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer yanlıştır. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Çalışma kitabının şifresini alır ve ayarlar. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. Varsayılan değer yanlıştır. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi adını ayarlar |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi boyutunu ayarlar. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // LoadOptions bir örnek oluşturur.
            LoadOptions loadOptions = new LoadOptions();

            // Özellikleri ayarlama
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Belirtilen LoadOptions ile bir çalışma kitabı yükleyin
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Çalışma kitabı üzerinde işlemler gerçekleştir.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Çalışma kitabını kaydedin
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


