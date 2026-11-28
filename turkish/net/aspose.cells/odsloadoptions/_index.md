---
title: "Class OdsLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.OdsLoadOptions sınıfı. ODS dosyası yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

ODS dosyasını yükleme seçeneklerini temsil eder.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OdsLoadOptions](odsloadoptions/#constructor)() | ODS dosyasını yükleme seçeneklerini temsil eder. |
| [OdsLoadOptions](odsloadoptions/#constructor_1)(LoadFormat) | ODS dosyasını yükleme seçeneklerini temsil eder. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/) { get; set; } | Excel'in varsayılan stilinin köprüye uygulanıp uygulanmayacağını gösterir. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Otomatik sığdırma seçeneklerini alır ve ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | workbook için stil başlatma varsayılan ayarlarını alır(Inherited from [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Bireysel font yapılandırmalarını alır ve ayarlar. Bu [`LoadOptions`](../loadoptions/) ile yüklenen [`Workbook`](../workbook/) için yalnızca çalışır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken basılmayan verileri yoksayar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Kullanışsız şekillerin yoksayılıp yoksayılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsClassicPivotTable](../../aspose.cells/odsloadoptions/isclassicpivottable/) { get; set; } | Özet tablonun klasik olup olmadığını gösterir. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Workbook için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirtir. Varsayılan true'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode'a dayalı olarak Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Verilerin nasıl yükleneceğini belirten filtre.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Yükleme biçimini alır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Yüklenen workbook için bellek modunu alır veya ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Workbook'un şifresini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Formülleri alırken ve ayarlarken formül belirteçleri arasına eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. (Miras alınan [`LoadOptions`](../loadoptions/).) |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables/) { get; set; } | Dosya yüklenirken özet tabloların yenilenip yenilenmeyeceğini gösterir. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi adını ayarlar(Miras alınan [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi boyutunu ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |
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

    public class OdsLoadOptionsDemo
    {
        public static void OdsLoadOptionsExample()
        {
            // OdsLoadOptions sınıfının bir örneğini oluşturun
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Özellikleri ayarlama
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            loadOptions.RefreshPivotTables = true;
            loadOptions.Password = "your_password";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new System.Globalization.CultureInfo("en-US");
            loadOptions.StandardFont = "Arial";
            loadOptions.StandardFontSize = 10.5;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.WarningCallback = new CustomWarningCallback();
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.FontConfigs = new IndividualFontConfigs();
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Belirtilen seçeneklerle bir ODS dosyası yükleyin
            Workbook workbook = new Workbook("OdsLoadOptionsExample_original.ods", loadOptions);

            // Çalışma kitabını yeni bir dosyaya kaydet
            workbook.Save("OdsLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


