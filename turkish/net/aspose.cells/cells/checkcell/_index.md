---
title: "Cells.CheckCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Belirtilen hücre satır indeksi ve sütun indeksindeki [`Cell`](../../cell/) öğesini veya null değerini alır.

```csharp
public Cell CheckCell(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |
| sütun | Int32 | Sütun indeksi |

### Dönüş Değeri

Bir Cell nesnesi mevcutsa Cell nesnesini döndür. Hücre mevcut değilse null döndür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelerdeki değerleri ayarla
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Int32 parametreleriyle CheckCell metodunu kullanarak hücreleri kontrol et
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Var olmayan hücreyi kontrol et (null dönecek)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


