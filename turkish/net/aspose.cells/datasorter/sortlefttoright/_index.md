---
title: "DataSorter.SortLeftToRight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. True, sıralama yönünün soldan sağa olduğunu gösterir. False, sıralama yönünün üstten alta olduğunu gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur.

```csharp
public bool SortLeftToRight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri (SortLeftToRight=true olduğunda sütunlar satır olarak ele alınır)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Veri sıralayıcı oluşturun ve soldan sağa sıralamayı ayarlayın
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Sıralama anahtarını ayarlayın (sütun indeksi, soldan sağa sıralama yapıldığında satır indeksine dönüşür)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Sıralama alanını tanımlayın (satırlar, soldan sağa sıralama yapıldığında sütunlara dönüşür)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Sıralamayı gerçekleştirin
            sorter.Sort(worksheet.Cells, area);

            // Sonucu kaydet
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


