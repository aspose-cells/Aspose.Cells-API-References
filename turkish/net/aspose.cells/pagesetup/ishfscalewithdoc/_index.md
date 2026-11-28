---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Üst bilgi ve alt bilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. Yalnızca Excel 2007 için geçerlidir"
type: docs
url: /tr/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Üst bilgi ve alt bilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. Yalnızca Excel 2007 için geçerlidir.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // Temel sayfa ayarlarını yap
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // IsHFScaleWithDoc özelliğini göster
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


