---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders özelliği. Çalışma sayfası dizini için önek"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Çalışma sayfası indeksinin öneki.

```csharp
public string SheetNamePrefix { get; set; }
```

### Açıklamalar

Eğer yalnızca bir çalışma sayfası varsa ve [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) false ise, bu önek ve çalışma sayfası dizini (veya adı) sonuç dosya yoluna eklenmez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Sağlayıcıyı sayfa yer tutucusu içeren yol şablonu ile başlat
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // İlk SheetNamePrefix değerini göster (varsayılan olarak boş)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Yeni önek ayarla ve yol oluşturmanın sayfa bilgilerini içerdiğinden emin ol
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Kaydetme seçeneklerini doğru formatta yapılandır
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Sağlayıcıyı kullanarak çalışma kitabını kaydet - "output_Q4_SalesData.xlsx" ve "output_Q4_FinancialReport.xlsx" dosyalarını oluşturur
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


