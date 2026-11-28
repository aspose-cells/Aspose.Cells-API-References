---
title: "Cells.ClearFormats"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir aralığın biçimlendirmesini temizler"
type: docs
url: /tr/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Bir aralığın biçimlendirmesini temizler.

```csharp
public void ClearFormats(CellArea range)
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

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Biçimlendirmeli örnek veri oluştur
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Hücrelere biçimlendirme uygula
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Temizleme alanını tanımla
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Orta hücreden biçimleri temizle
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Etkiyi göstermek için temizlenen hücre değerini güncelle
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Sonucu kaydedin
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
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

## ClearFormats(int, int, int, int) {#clearformats_1}

Bir aralığın biçimlendirmesini temizler.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı hücrelere stil uygula
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Belirli bir aralıktaki (satırlar 5-15, sütunlar 5-15) biçimleri temizle
            cells.ClearFormats(5, 5, 15, 15);

            // Çalışma kitabını kaydedin
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


