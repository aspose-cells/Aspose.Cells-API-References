---
title: "DataSorter.Key2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. İkinci sıralanan sütun indeksini temsil eder; mutlak konum: sütun A 0, B 1"
type: docs
url: /tr/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

İkinci sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

```csharp
public int Key2 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // DataSorter oluştur ve özellikleri ayarla
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Veri aralığını sırala
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Key2 kullanımını göstermek için sıralanmış veriyi çıktı al
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


