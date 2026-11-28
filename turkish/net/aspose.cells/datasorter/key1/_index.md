---
title: "DataSorter.Key1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. İlk sıralanan sütun indeksini temsil eder; mutlak konum, sütun A 0, B 1'dir."
type: docs
url: /tr/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

İlk sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

```csharp
public int Key1 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin.
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Veri sıralayıcı oluşturun ve Key1'i Score sütununa göre (sütun B) sıralamak için ayarlayın
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Sıralama alanını tanımlayın (satırlar 1-4, tüm veri sütunları)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Sıralamayı gerçekleştirin
            sorter.Sort(cells, sortArea);

            // Sonucu kaydet
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


