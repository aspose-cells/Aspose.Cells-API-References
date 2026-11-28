---
title: "Enum SortOrder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SortOrder enum. Veri aralığı için sıralama düzenini temsil eder"
type: docs
url: /tr/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Veri aralığı için sıralama düzenini temsil eder.

```csharp
public enum SortOrder
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Ascending | `0` | Verileri artan sırada sıralar |
| Descending | `1` | Verileri azalan sırada sıralar |
| Natural | `2` | Sıralama yapmadan orijinal veri sırasını korur. Yalnızca PivotTable gibi bazı özel senaryolara uygulanır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            var workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sıralamak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Veri sıralayıcı oluştur
            var sorter = workbook.DataSorter;
            
            // Sıralama düzenini ve anahtarları ayarla
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Sıralama alanını tanımla
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Sıralamayı gerçekleştirin
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


