---
title: "Worksheet.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfası tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Çalışma sayfası tipini temsil eder.

```csharp
public SheetType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı temel özellikleri ayarla
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Type özelliğinin kullanımını gösterin.
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Farklı çalışma sayfası tipini göstermek için bir chart sheet ekle
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Çalışma sayfası tiplerini karşılaştır
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


