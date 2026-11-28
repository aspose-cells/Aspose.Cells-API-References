---
title: "Worksheet.IsOutlineShown"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Taslağın gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Anahatın gösterilip gösterilmeyeceğini gösterir.

```csharp
public bool IsOutlineShown { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Taslağın gösterilmesini ayarlayın
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Kalıcılığı göstermek için kaydedin ve yeniden yükleyin
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


