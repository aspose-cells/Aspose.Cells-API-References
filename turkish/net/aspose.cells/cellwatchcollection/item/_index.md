---
title: "CellWatchCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellWatchCollection özelliği. CellWatch'ı indeksle alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

[`CellWatch`](../../cellwatch/) öğesini indeksle alır ve ayarlar.

```csharp
public CellWatch this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Item özelliğinin kullanımını göster
            CellWatch cellWatch = cellWatches[watchIndex];
            
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A1";
            
            Console.WriteLine("\nModified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            workbook.Save("CellWatchCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

[`CellWatch`](../../cellwatch/) öğesini hücrenin adıyla alır ve ayarlar.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücrenin adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Koleksiyona bir hücre izleyici ekle
                int watchIndex = worksheet.CellWatches.Add("A1");

                // CellWatchCollection'a eriş
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // İndeksleyici kullanarak Item özelliğine erişimi göster
                CellWatch cellWatch = cellWatches[watchIndex];

                // CellWatch öğesinin özelliklerini göster
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Çalışma kitabını kaydedin
                workbook.Save("CellWatchItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


