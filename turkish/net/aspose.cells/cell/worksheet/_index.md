---
title: "Cell.Worksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Üst çalışma sayfasını alır"
type: docs
url: /tr/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Üst çalışma sayfasını alır.

```csharp
public Worksheet Worksheet { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Bir hücreye erişin ve Worksheet özelliğini gösterin
            Cell cell = worksheet.Cells["A3"];
            
            // Hücrenin Worksheet özelliği aracılığıyla çalışma sayfası bilgilerini gösterin
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Başka bir çalışma sayfası ekleyin ve sayfalar arası referansı gösterin
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Sheet2'deki hücreye erişin ve onun çalışma sayfasını gösterin
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


