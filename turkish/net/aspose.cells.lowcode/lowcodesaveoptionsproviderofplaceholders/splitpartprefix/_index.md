---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders özelliği. Bölünmüş parçanın dizini için önek"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

Bölünmüş parça indeksinin öneki.

```csharp
public string SplitPartPrefix { get; set; }
```

### Açıklamalar

Yalnızca bir bölünmüş parça varsa ve [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) false ise, bu önek ve bölünmüş parça indeksi (0) sonuç dosya yoluna eklenmez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Kaydetme seçenekleri şablonunu yapılandır.
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // Sağlayıcıyı bölünmüş parça yer tutucusu ile başlat
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // SplitPartPrefix'i göster ve değiştir
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Sağlayıcının kaydetme formatını kullanarak çalışma kitabını bölünmüş parçalarla kaydet
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


