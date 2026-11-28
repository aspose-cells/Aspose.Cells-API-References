---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Sütun genişliğinin ölçek biriminde HTML'ye aktarılıp aktarılmayacağını gösterir. Varsayılan değer false."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Sütun genişliğinin ölçek birimi olarak HTML'ye dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false.

```csharp
public bool WidthScalable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // WidthScalable özelliği ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Ölçeklenebilir genişlikle kaydedin
            workbook.Save("output_scalable.html", options);
            
            // Sabit genişlikle tekrar kaydedin
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


