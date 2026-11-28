---
title: "Worksheet.ActiveCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki aktif hücreyi alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Çalışma sayfasındaki aktif hücreyi alır veya ayarlar.

```csharp
public string ActiveCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aktif hücreyi B2'ye ayarlayın
            worksheet.ActiveCell = "B2";
            
            // Etkin hücre adresini yazdır
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek etkin hücreyi doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


