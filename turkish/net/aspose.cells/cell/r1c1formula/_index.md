---
title: "Cell.R1C1Formula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin R1C1 formülünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

[`Cell`](../) nesnesinin R1C1 formülünü alır veya ayarlar.

```csharp
public string R1C1Formula { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 değerini ayarla
            worksheet.Cells["A1"].PutValue(10);
            
            // B1 değerini ayarla
            worksheet.Cells["B1"].PutValue(20);
            
            // C1 formülünü A1 notasyonunda ayarla
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // R1C1 formülünü al ve göster
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // D1 formülünü R1C1 notasyonunda ayarla
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // A1 formülünü al ve göster
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


