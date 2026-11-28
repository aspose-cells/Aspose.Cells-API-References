---
title: "DataSorter.CaseSensitive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. Dize karşılaştırılırken büyük/küçük harf duyarlılığını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır ve ayarlar.

```csharp
public bool CaseSensitive { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı ve çalışma sayfası oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Büyük/küçük harf varyasyonlarıyla örnek veri ekle
            cells["A1"].PutValue("apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("banana");
            cells["A4"].PutValue("APPLE");
            cells["A5"].PutValue("orange");
            cells["A6"].PutValue("Banana");

            // Veri sıralayıcı oluştur
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by first column
            sorter.Order1 = SortOrder.Ascending;

            // Büyük/küçük harf duyarlı sıralamayı göster
            Console.WriteLine("Sorting with CaseSensitive = true:");
            sorter.CaseSensitive = true;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");

            // Büyük/küçük harf duyarsız sıralamayı göster
            Console.WriteLine("\nSorting with CaseSensitive = false:");
            sorter.CaseSensitive = false;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");
        }

        private static void PrintSortedData(Cells cells, string range)
        {
            Console.WriteLine("Sorted data:");
            foreach (Cell cell in cells.CreateRange(range))
            {
                Console.WriteLine(cell.StringValue);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


