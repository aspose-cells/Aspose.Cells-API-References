---
title: "Worksheet.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının görünür olup olmadığını temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Çalışma sayfasının görünür olup olmadığını temsil eder.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // 3 çalışma sayfası ekle
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // İkinci çalışma sayfasını gizli olarak ayarla
            workbook.Worksheets[1].IsVisible = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Görünürlük durumunu göster
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


