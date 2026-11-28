---
title: "Enum ViewType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ViewType enum. Çalışma sayfasının görünüm türünü temsil eder."
type: docs
url: /tr/net/aspose.cells/viewtype/
---
## ViewType enumeration

Çalışma sayfasının görünüm türünü temsil eder.

```csharp
public enum ViewType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının görünüm türünü PageBreakPreview olarak ayarla
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


