---
title: "Worksheet.IsSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma kitabı açıldığında bu çalışma sayfasının seçili olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Çalışma kitabı açıldığında bu çalışma sayfasının seçili olup olmadığını gösterir.

```csharp
public bool IsSelected { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İkinci bir çalışma sayfası ekle
            workbook.Worksheets.Add("Sheet2");
            
            // İlk çalışma sayfasını al
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // İkinci çalışma sayfasını al
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // IsSelected özelliğini göster
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // İkinci çalışma sayfasını seç
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


