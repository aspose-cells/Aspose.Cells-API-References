---
title: "Sınıf DataSorterKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataSorterKey sınıfı. Veri sıralayıcının anahtarını temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Veri sıralayıcının anahtarını temsil eder.

```csharp
public class DataSorterKey
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Sıralanmış rengi alır. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Simge seti türünün kimliğini temsil eder. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Simge seti türünü temsil eder. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Sıralanmış sütun indeksini alır (mutlak konum, A sütunu 0, B 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Sıralama düzenini gösterir. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Sıralama türünü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Bir çalışma kitabı nesnesi oluşturun ve bir şablon dosyası yükleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sıralanacak örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Veri sıralayıcı nesnesini örnekleyin
            DataSorter sorter = workbook.DataSorter;

            // İlk sütun (A) için artan sırada sıralama anahtarı ekleyin
            sorter.AddKey(0, SortOrder.Ascending);

            // Sıralanacak bir hücre alanı (aralık) oluşturun
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Sıralamayı gerçekleştirin
            sorter.Sort(worksheet.Cells, ca);

            // Çıktı dosyasını kaydedin
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // DataSorterKeyCollection'a erişin
            DataSorterKeyCollection keys = sorter.Keys;

            // Anahtarlar üzerinde döngü yapın ve özelliklerini yazdırın
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


