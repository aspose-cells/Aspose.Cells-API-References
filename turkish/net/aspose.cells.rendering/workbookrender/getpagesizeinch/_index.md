---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookRender yöntemi. Çıktı görüntüsünün inç cinsinden sayfa boyutunu alır"
type: docs
url: /tr/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

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

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


