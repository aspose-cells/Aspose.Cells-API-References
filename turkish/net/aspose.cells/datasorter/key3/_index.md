---
title: "DataSorter.Key3"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. Üçüncü sıralanan sütun indeksini temsil eder, mutlak konum: sütun A 0, B 1"
type: docs
url: /tr/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Üçüncü sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

```csharp
public int Key3 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin.
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Veri sıralayıcı oluştur
            DataSorter sorter = workbook.DataSorter;
            
            // Score (azalan), ardından Name (artan), ardından Grade (azalan) sırasıyla sırala
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Veri aralığını sırala
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Çalışma kitabını kaydedin
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


