---
title: "DataSorter.Order1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. İlk anahtarın sıralama düzenini temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

İlk anahtarın sıralama düzenini temsil eder.

```csharp
public SortOrder Order1 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Veri sıralayıcı özelliklerini ayarla
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Sıralama aralığını tanımla
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Sıralamayı gerçekleştirin
            sorter.Sort(worksheet.Cells, area);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


