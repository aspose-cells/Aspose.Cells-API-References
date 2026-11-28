---
title: "Enum PageOrientationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PageOrientationType enum. Yazdırma yönlendirme sabitlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Yazdırma yönü sabitlerini temsil eder.

```csharp
public enum PageOrientationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Landscape | `0` | Yatay yön |
| Portrait | `1` | Dikey yön |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının PageSetup nesnesine erişin
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Sayfa yönünü Yatay olarak ayarlayın
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Sayfa yönünü Dikey olarak ayarlayın
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Çalışma kitabını farklı bir dosyaya kaydedin
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


