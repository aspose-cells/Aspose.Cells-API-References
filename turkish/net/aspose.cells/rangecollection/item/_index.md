---
title: "RangeCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RangeCollection özelliği. Belirtilen dizindeki Range öğesini alır"
type: docs
url: /tr/net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

Belirtilen dizindeki [`Range`](../../range/) öğesini alır.

```csharp
public Range this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı aralıklar oluştur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Aralıkları koleksiyona ekle
            RangeCollection ranges = worksheet.Cells.Ranges;
            ranges.Add(range1);
            ranges.Add(range2);
            ranges.Add(range3);

            // Item özelliğinin kullanımını göster
            Console.WriteLine("Range Collection Count: " + ranges.Count);
            for (int i = 0; i < ranges.Count; i++)
            {
                Aspose.Cells.Range currentRange = ranges[i]; // Using Item property
                Console.WriteLine($"Range {i + 1}: {currentRange.Address}");
                Console.WriteLine($"  - FirstRow: {currentRange.FirstRow}");
                Console.WriteLine($"  - FirstColumn: {currentRange.FirstColumn}");
                Console.WriteLine($"  - RowCount: {currentRange.RowCount}");
                Console.WriteLine($"  - ColumnCount: {currentRange.ColumnCount}");
            }

            // Belirli bir aralığa dizinle eriş
            Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
            Console.WriteLine("\nSecond range details:");
            Console.WriteLine($"Address: {secondRange.Address}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


