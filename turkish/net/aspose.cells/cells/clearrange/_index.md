---
title: "Cells.ClearRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir aralığın içeriğini ve biçimlendirmesini temizler"
type: docs
url: /tr/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Bir aralığın içeriğini ve biçimlendirmesini temizler.

```csharp
public void ClearRange(CellArea range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | CellArea | Temizlenecek aralık. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücreleri örnek veriyle doldurun
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Temizlenecek CellArea'yi tanımlayın (satırlar 0-2, sütunlar 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Belirtilen aralığı temizle
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Bir aralığın içeriğini ve biçimlendirmesini temizler.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| startColumn | Int32 | Başlangıç sütun indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |
| endColumn | Int32 | Bitiş sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Bazı test verileri doldurun
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Tüm çalışma sayfası aralığını temizle
            cells.ClearRange(0, 0, 1048575, 16383);

            // Çalışma kitabını kaydedin
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


