---
title: "CellWatchCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellWatchCollection yöntemi. Bir satır ve sütun ile CellWatch ekler"
type: docs
url: /tr/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Bir satır ve sütun ile [`CellWatch`](../../cellwatch/) ekler.

```csharp
public int Add(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

Bu öğenin koleksiyondaki konumunu döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından CellWatchCollection'ı alın
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Satır ve sütun indeksleri (Int32, Int32) ile Add metodunu çağırın
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Eklenen hücre izleyiciyi doğrulayın
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Hücrenin adıyla [`CellWatch`](../../cellwatch/) ekler.

```csharp
public int Add(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücrenin adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı hücre izlemeleri ekle
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Hücre izleyicilerin sayısını göster
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


