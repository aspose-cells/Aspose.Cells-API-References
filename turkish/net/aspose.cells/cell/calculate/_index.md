---
title: "Cell.Calculate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücrenin formülünü hesaplar"
type: docs
url: /tr/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Hücrenin formülünü hesaplar.

```csharp
public void Calculate(CalculationOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | CalculationOptions | Hesaplama seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine basit bir formül ayarla
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Varsayılan seçeneklerle hesapla
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // B1:D1 aralığına bir dizi formülü ayarla
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Seçeneklerle dizi formülünü hesapla
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // A2 hücresine daha karmaşık bir formül ayarla
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Seçeneklerle hesapla
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


