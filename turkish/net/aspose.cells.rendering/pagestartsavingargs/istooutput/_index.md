---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageStartSavingArgs özelliği. Sayfanın çıktıya alınması gerekip gerekmediğini gösteren bir değeri alır veya ayarlar. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Sayfanın çıktılanıp çıktılanmayacağını gösteren değeri alır veya ayarlar. Varsayılan değer doğrudur.

```csharp
public bool IsToOutput { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Birden fazla sayfa oluşturmak için verileri doldurun
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Düzeltildi: Satır yüksekliğine çalışma sayfasının Rows koleksiyonu aracılığıyla erişin
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Geçerli değeri oku
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Her çift numaralı sayfayı atla (1 tabanlı numaralandırma)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Bu gösterim için uygulama gerekli değil
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


