---
title: "SheetRender.PageScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender özelliği. Sayfanın hesaplanan sayfa ölçeğini alır. Zoom ayarlanmışsa ayarlanan ölçeği döndürür. Aksi takdirde FitToPagesWide ve FitToPagesTall değerlerine göre hesaplanan ölçeği döndürür."
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Sayfanın hesaplanan sayfa ölçeğini alır. [`Zoom`](../../../aspose.cells/pagesetup/zoom/) ayarlanmışsa ayarlanan ölçeği döndürür. Aksi takdirde, [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) ve [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/) değerlerine göre hesaplanan ölçeği döndürür.

```csharp
public double PageScale { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Görüntü veya yazdırma seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Sheet render oluşturun
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Hesaplanan sayfa ölçeğini alın ve görüntüleyin
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


