---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Aralığın silinebilir olup olmadığını kontrol edin"
type: docs
url: /tr/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Aralığın silinebileceğini kontrol eder.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Aralığın başlangıç satır indeksi. |
| startColumn | Int32 | Aralığın başlangıç sütun indeksi. |
| totalRows | Int32 | Aralıktaki satır sayısı. |
| totalColumns | Int32 | Aralıktaki sütun sayısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // A1:C5 hücrelerine örnek veri doldurun
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // A1'den başlayan 5 satır x 3 sütun silmenin etkin olup olmadığını kontrol edin
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // A1:C5 aralığını sil ve hücreleri yukarı kaydır
                    cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
                    Console.WriteLine("Deleted range A1:C5 successfully");
                }

                workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during range deletion: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


