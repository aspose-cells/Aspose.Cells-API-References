---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IPageSavingCallback yöntemi. Çıktıya bir sayfanın sonlandığını kontrol/indike eder"
type: docs
url: /tr/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Çıktıya bir sayfanın sonlandığını kontrol/indike eder.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | PageEndSavingArgs | Bir sayfa için bilgi, kaydetme sürecini sonlandırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve verileri doldur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Render edildiğinde birden fazla sayfa oluşturmak için örnek veri ekle
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Özel sayfa kaydetme geri çağrımıyla PDF kaydetme seçeneklerini oluştur
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Geri çağrı uygulamasıyla çalışma kitabını kaydet
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Sayfa kaydetme tamamlanma bilgisini göster
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Burada dosya işlemleri veya diğer son işlemeleri ekleyebilirsiniz
                // args.HasMorePages daha fazla sayfanın işleneceğini gösterir
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Gerekli arayüz uygulaması
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


