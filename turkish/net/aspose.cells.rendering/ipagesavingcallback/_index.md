---
title: "Arayüz IPageSavingCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.IPageSavingCallback arayüzü. Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder"
type: docs
url: /tr/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Sayfa kaydetme işleminin ilerlemesini kontrol/indike eder.

```csharp
public interface IPageSavingCallback
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Çıktıya bir sayfanın sonlandığını kontrol/indike eder. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Çıktıya bir sayfanın başladığını kontrol/indike eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Sayfa kaydetme geri çağrısı ile kaydetme seçenekleri oluştur
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Çalışma kitabını DOCX dosyası olarak kaydet
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // PageStartSaving metodunu uygula
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // PageEndSaving metodunu uygula
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


