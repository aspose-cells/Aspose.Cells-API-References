---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeHtmlSaveOptions özelliği. HTML kaydetme için genel seçenekler"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

HTML kaydetme için genel seçenekler.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Açıklamalar

Bir [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) örneği belirtildiğinde, [`SaveFormat`](../saveformat/) üzerine yazılacak (daha önce belirtilmişse).

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Düşük kodlu HTML kaydetme seçenekleri oluştur
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Mevcut ızgara çizgileri dışa aktarma ayarını göster
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Izgara çizgileri görünür olarak kaydet
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // HTML seçeneklerini ızgara çizgilerini gizleyecek şekilde değiştir
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Izgara çizgileri olmadan kaydet
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


