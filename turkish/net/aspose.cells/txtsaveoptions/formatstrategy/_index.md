---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Hücre değerini dize olarak dışa aktarırken format stratejisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

Hücre değerini dize olarak dışa aktarırken format stratejisini alır ve ayarlar.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı formatlarla değerleri ayarla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Fiyatlara sayı formatı uygula
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Farklı format stratejileriyle metin kaydetme seçeneklerini yapılandır
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Görüntüleme formatı ile kaydet
            workbook.Save("FormattedOutput.txt", options);

            // Biçimlendirme stratejisi olmadan değiştir
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


