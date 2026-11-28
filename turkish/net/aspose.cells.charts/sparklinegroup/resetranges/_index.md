---
title: "SparklineGroup.ResetRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup yöntemi. Sparkline grubunun veri aralığını ve konum aralığını sıfırlar. Bu yöntem, gruptaki orijinal sparkline öğelerini temizleyecek ve yeni aralıklar için yeni sparkline öğeleri oluşturacaktır"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Sparkline grubunun veri aralığını ve konum aralığını sıfırlar. Bu yöntem, gruptaki orijinal sparkline öğelerini temizler ve yeni aralıklar için yeni sparkline öğeleri oluşturur.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataRange | String | Sparkline grubunun yeni veri aralığını belirtir. |
| isVertical | Boolean | Yeni veri aralığından sparklineları satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| locationRange | CellArea | Sparklineların nereye yerleştirileceğini belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline için CellArea'yı tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Çalışma sayfasına bir sparkline grubu ekle
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            SparklineGroup group = sheet.SparklineGroups[idx];

            // ResetRanges için parametreleri hazırlayın
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // ResetRanges'i (String, Boolean, CellArea) parametreleriyle çağırın
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


