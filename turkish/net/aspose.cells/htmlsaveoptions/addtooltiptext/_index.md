---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Veriler tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur.

```csharp
public bool AddTooltipText { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre genişliğini aşacak uzun bir metin ayarlayın
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // Araç ipucu ile HTML kaydetme seçeneklerini yapılandırın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // Çalışma kitabını kaydedin
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


