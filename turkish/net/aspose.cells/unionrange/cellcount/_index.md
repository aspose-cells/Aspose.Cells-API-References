---
title: "UnionRange.CellCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralıktaki toplam hücre sayısını alır"
type: docs
url: /tr/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

Aralıktaki tüm hücre sayısını alır.

```csharp
public int CellCount { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına veri doldurun
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // Aralıklar oluşturun ve bunları bir birleşim aralığına birleştirin
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // CellCount özelliğini göster
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // Beklenen hücre sayısını hesaplayın
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // Hücreler üzerinde döngü yaparak kullanımını gösterin
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // Hücre sayısının yineleme ile eşleştiğini doğrulayın
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // Farklı boyutlarla başka bir birleşim aralığı oluşturun
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // Farklı birleşim aralıklarının hücre sayılarını karşılaştırın
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


