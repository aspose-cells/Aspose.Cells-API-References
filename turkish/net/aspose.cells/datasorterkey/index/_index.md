---
title: "DataSorterKey.Index"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKey özelliği. Sıralanmış sütun indeksini alır, mutlak konum: sütun A 0, B 1"
type: docs
url: /tr/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Sıralanmış sütun indeksini alır (mutlak konum, A sütunu 0, B 1, ...).

```csharp
public int Index { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sıralamak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Veri sıralayıcı oluştur ve sıralama anahtarı ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Index özelliğinin kullanımını göster
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Sonucu kaydet
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


