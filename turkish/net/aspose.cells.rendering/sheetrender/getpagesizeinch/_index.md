---
title: "SheetRender.GetPageSizeInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender yöntemi. Çıktı görüntüsünün sayfa boyutunu inç olarak alın"
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Çıktı görüntüsünün inç cinsinden sayfa boyutunu al.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | Sayfa indeksi sıfır temelli olarak belirlenir. |

### Dönüş Değeri

Görüntünün sayfa boyutu, [0] genişlik ve [1] yükseklik için

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


