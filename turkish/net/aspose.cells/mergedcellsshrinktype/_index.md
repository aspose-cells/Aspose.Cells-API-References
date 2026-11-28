---
title: "Enum MergedCellsShrinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.MergedCellsShrinkType enum. Birleştirilmiş hücreleri boş satır/sütunları silme gibi işlemler için küçültme stratejisini temsil eder"
type: docs
url: /tr/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Boş satır/sütunları silme gibi işlemler için birleştirilmiş hücreleri küçültme stratejisini temsil eder.

```csharp
public enum MergedCellsShrinkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Birleştirilmiş hücreleri herhangi bir değişiklik yapmadan olduğu gibi bırakır. |
| ShrinkToFit | `1` | Gerekirse, alt taraftan satırları veya sağ taraftan sütunları kaldırarak birleştirilmiş alanı küçültür ve tüm içeriğin görünür kalmasını sağlar. |
| KeepHeaderOnly | `2` | Birleştirilmiş alanın sol üst hücresi boş olmadığında yalnızca başlık satırlarını/sütunlarını tutar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Birleştirilmiş hücrelerle örnek veriyi başlat
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Seçenek 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Çalışma sayfasını sıfırla
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Seçenek 2: None
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Çalışma sayfasını sıfırla
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Seçenek 3: ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


