---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders özelliği. Çalışma sayfası dizini için önek"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Çalışma sayfası indeksinin öneki.

```csharp
public string SheetIndexPrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Birden fazla çalışma sayfasına sahip yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // LowCodeSaveOptionsProviderOfPlaceHolders örneği oluştur
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // SheetIndexPrefix'i görüntüleyin ve değiştirin
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Diğer gerekli özellikleri ayarlayın
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // SheetIndexPrefix'in dosya yolları üzerindeki etkisini gösterin
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // SplitPartInfo'yi doğrudan oluşturup dolduramıyoruz,
                // onun olmadan sadece adlandırma desenini göstereceğiz
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Adlandırma desenini göstermek için çalışma kitabını kaydedin
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


