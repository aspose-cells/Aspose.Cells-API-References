---
title: "Cells.ClearMergedCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm birleştirilmiş aralıkları temizler"
type: docs
url: /tr/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Tüm birleştirilmiş aralıkları temizler.

```csharp
public void ClearMergedCells()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1:B2 aralığında birleştirilmiş hücreler oluştur
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Çalışma sayfasındaki tüm birleştirilmiş hücreleri temizle
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


