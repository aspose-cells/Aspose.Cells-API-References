---
title: "DataSorter.SortAsNumber"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. Sayıya benzeyen her şeyi sıralayıp sıralamayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Sıralamanın sayı gibi görünen şeyleri içerip içermediğini gösterir.

```csharp
public bool SortAsNumber { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karışık sayılar ve metin sayılarıyla örnek veri ekle
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Sıralanacak hücre alanı oluştur
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Veri sıralayıcı oluştur
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Sıralama anahtarı ekle (A sütunu)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Sayı olarak sırala (true) ya da dize olarak (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // İkinci sıralama için veriyi sıfırla
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Dize olarak sırala
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


