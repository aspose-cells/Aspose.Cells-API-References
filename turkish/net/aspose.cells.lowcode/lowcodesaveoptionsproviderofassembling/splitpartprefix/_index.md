---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling property. Bölünmüş parçanın indeksinin öneki"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

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
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Birden fazla sayfaya yayılan verilerle çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Birden fazla sayfa oluşturmak için sayfa ayarlarını yapılandırın
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Split yapılandırmasıyla kaydetme seçenekleri sağlayıcısını başlatın
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // İlk önekle kaydedin (SplitResults/OriginalPart_0.pdf vb. oluşturulacak)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Split önekini değiştirin
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Değiştirilmiş önekle kaydedin (SplitResults/ModifiedPart_0.pdf vb. oluşturulacak)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


