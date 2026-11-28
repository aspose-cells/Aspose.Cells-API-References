---
title: "Range.RowCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralıktaki satır sayısını alır"
type: docs
url: /tr/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Aralıktaki satır sayısını alır.

```csharp
public int RowCount { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1:B10 hücrelerinde örnek veri oluşturun
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // A1:B10 aralığını kapsayan adlandırılmış bir aralık oluşturun
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Adlandırılmış aralığı al
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // RowCount özelliğini göster
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


