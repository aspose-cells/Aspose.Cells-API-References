---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling property. Dosya yolunda kullanılan sayfa indeksi ile gerçek değeri (SheetIndex) arasındaki ofset"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Dosya yolunda kullanılan sayfa indeksi ile gerçek değeri ([`SheetIndex`](../../splitpartinfo/sheetindex/)) arasındaki ofset.

```csharp
public int SheetIndexOffset { get; set; }
```

### Açıklamalar

Yalnızca [`UseSheetName`](../usesheetname/) false olduğunda etkili olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Kaydetme seçenekleri sağlayıcısını başlat
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Orijinal ofseti göster
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // İlk ofsetle kaydet (sayfalar 10 ve 11 olarak numaralanacak)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Ofseti değiştir ve tekrar kaydet
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Yeni ofsetle kaydet (sayfalar 100 ve 101 olarak numaralanacak)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


