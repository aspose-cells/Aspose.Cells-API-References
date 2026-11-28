---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders özelliği. Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir sayfa olduğunda sayfa indeksi, adı ve ilgili prefixSheetNamePrefix dosya yoluna eklenmez."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda sayfa indeksi, adı ve ilgili prefix([`SheetNamePrefix`](../sheetnameprefix/)) dosya yoluna eklenmez.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Yol farklarını göstermek için iki sayfalı bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Sağlayıcıyı sayfa indeksi yer tutucusuyla yapılandır
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Sayfa indeksi offsetini (isteğe bağlı) göster
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Birden fazla sayfa olduğunda yalnızca sayfa indeksiyle kaydet (varsayılan davranış)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Tek sayfalar için bile dosya adlarında sayfa indeksini zorla
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Bölmeyi etkinleştirmek için JSON formatında kaydetme seçeneklerini yapılandır
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Sağlayıcıyı kaydetme seçenekleriyle yapılandır
            provider.SaveOptionsTemplate = saveOptions;

            // Sağlayıcı tarafından belirlenen yollarla kaydet
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


