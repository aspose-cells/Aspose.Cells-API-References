---
title: "Range.Transpose"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Transpose, verileri satırlardan sütunlara veya tersine döndürür"
type: docs
url: /tr/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Verileri satırlardan sütunlara veya tersine (döndür) transpoze et.

```csharp
public void Transpose()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 3x3 bir aralıkta (A1:C3) örnek veri doldur
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Bir aralık oluştur (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Aralığı transpoze et
            range.Transpose();
            
            // Çalışma kitabını kaydedin
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


