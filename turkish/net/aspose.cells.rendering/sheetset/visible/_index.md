---
title: "SheetSet.Visible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetSet özelliği. Çalışma kitabının görünür sayfalarını orijinal sırasıyla içeren bir küme alır"
type: docs
url: /tr/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Çalışma kitabının görünür sayfalarını orijinal sıralarında içeren bir set alır.

```csharp
public static SheetSet Visible { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // İkinci çalışma sayfasını gizle
            workbook.Worksheets[1].IsVisible = false;

            // Yalnızca görünür sayfaları dışa aktarmak için kaydetme seçeneklerini ayarlayın
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Çalışma kitabını kaydedin (yalnızca görünür sayfa dışa aktarılacak)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


