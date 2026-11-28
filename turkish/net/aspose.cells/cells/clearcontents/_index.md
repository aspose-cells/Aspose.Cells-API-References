---
title: "Cells.ClearContents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir aralığın içeriğini temizler"
type: docs
url: /tr/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Bir aralığın içeriğini temizler.

```csharp
public void ClearContents(CellArea range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | CellArea | Temizlenecek aralık. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Bir hücre alanına bazı verileri doldur
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Hücre alanının içeriğini temizle
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
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

## ClearContents(int, int, int, int) {#clearcontents_1}

Bir aralığın içeriğini temizler.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı hücreleri değerlerle doldur
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Orijinal değerleri göster
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // (0,1) ile (1,1) arasındaki hücrelerin içeriğini temizle
            cells.ClearContents(0, 1, 1, 1);

            // Temizledikten sonra değerleri göster
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Çalışma kitabını kaydedin
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


