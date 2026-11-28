---
title: "DeleteBlankOptions.EndIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteBlankOptions özelliği. Kontrol edilecek ve boş satır/sütunları silmek için aralığın son satır/sütun indeksini belirtir. Varsayılan değer 1'dir ve 1, kontrol edilmesi gereken tüm nesneler, hücreler, çizimler ... için maksimum aralığı ifade eder."
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Kontrol edilecek ve boş satırları/sütunları silinecek aralığın son satır/sütun indeksini (dahil) belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder.

```csharp
public int EndIndex { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Bazı hücreleri değerlerle doldur
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Belirli bir aralıkla silme seçenekleri oluştur
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Belirtilen aralık içinde boş sütunları sil
            cells.DeleteBlankColumns(dbo);

            // EndIndex etkisini göstermek için sonuçları çıktı al
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


