---
title: "Enum ConsolidationFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ConsolidationFunction enum. Birleştirme işlevini temsil eder"
type: docs
url: /tr/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Konsolidasyon işlevini temsil eder.

```csharp
public enum ConsolidationFunction
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Sum | `0` | Sum işlevini temsil eder. |
| Count | `1` | Count işlevini temsil eder. |
| Average | `2` | Average işlevini temsil eder. |
| Max | `3` | Max işlevini temsil eder. |
| Min | `4` | Min işlevini temsil eder. |
| Product | `5` | Product işlevini temsil eder. |
| CountNums | `6` | Count Nums işlevini temsil eder. |
| StdDev | `7` | StdDev işlevini temsil eder. |
| StdDevp | `8` | StdDevp işlevini temsil eder. |
| Var | `9` | Var işlevini temsil eder. |
| Varp | `10` | Varp işlevini temsil eder. |
| DistinctCount | `11` | Distinct Count işlevini temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Alt toplam için hücre alanını tanımla
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Sum işleviyle alt toplamı uygula
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Average işleviyle alt toplamı uygula
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Max işleviyle alt toplamı uygula
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Min işleviyle alt toplamı uygula
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Çalışma kitabını kaydedin
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


