---
title: "DataSorter.HasHeaders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. Aralığın başlık içerip içermediğini temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Aralığın başlık içerip içermediğini temsil eder.

```csharp
public bool HasHeaders { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Başlıkları ve örnek verileri ekle
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Veri sıralayıcı oluştur ve HasHeaders'ı true olarak ayarla
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // İlk sütuna (Meyveler) göre artan sırada sırala
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Veri aralığını sırala (başlıklar dahil)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Sıralanmış çalışma kitabını kaydet
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


