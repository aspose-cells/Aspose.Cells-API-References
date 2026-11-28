---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Izgara çizgi rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Izgara çizgi rengini alır veya ayarlar.

```csharp
public Color GridlineColor { get; set; }
```

### Açıklamalar

Kaynak dosyadaki ızgara çizgi rengi ayarlarını yok sayacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // PDF kaydetme seçeneklerini oluşturun
                PdfSaveOptions options = new PdfSaveOptions();

                // Varsayılan GridlineColor değerini gösterin
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Yeni bir ızgara çizgi rengi ayarlayın
                options.GridlineColor = Color.Red;

                // Güncellenmiş GridlineColor değerini gösterin
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Izgara çizgi rengi ayarıyla çalışma kitabını kaydedin
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


