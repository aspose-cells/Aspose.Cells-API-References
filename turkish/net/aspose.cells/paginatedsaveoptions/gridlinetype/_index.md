---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Gridline tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

Izgara çizgi tipini alır veya ayarlar.

```csharp
public GridlineType GridlineType { get; set; }
```

### Açıklamalar

Varsayılan Dotted tipidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekle ve ızgaraları etkinleştir
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // GridlineType özelliğini göster
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // Çalışma kitabını ızgaralarla kaydet
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


