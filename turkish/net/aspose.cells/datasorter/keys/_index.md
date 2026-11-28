---
title: "DataSorter.Keys"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter özelliği. Veri sıralayıcının anahtar listesini alır"
type: docs
url: /tr/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Veri sıralayıcısının anahtar listesini alır.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Veri sıralayıcıyı başlat
            DataSorter sorter = workbook.DataSorter;
            
            // Sütun A (indeks 0) için sıralama anahtarı ekle
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Keys özelliğinin kullanımını göster
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


