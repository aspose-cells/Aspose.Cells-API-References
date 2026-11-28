---
title: "SheetSet.Active"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetSet özelliği. Çalışma kitabının aktif sayfasını içeren bir küme alır"
type: docs
url: /tr/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Çalışma kitabının aktif sayfasını içeren bir set alır.

```csharp
public static SheetSet Active { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // İkinci çalışma sayfasını aktif olarak ayarlayın
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Her iki çalışma sayfasına da veri ekleyin
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Yalnızca aktif sayfayı kaydedin
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Karşılaştırma için tüm sayfaları kaydedin
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


