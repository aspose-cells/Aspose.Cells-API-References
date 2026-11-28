---
title: "Cells.CheckRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücre satır indeksinde Row öğesini veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Belirtilen hücre satır indeksinde [`Row`](../../row/) öğesini veya null değerini alır.

```csharp
public Row CheckRow(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |

### Dönüş Değeri

Satır nesnesi mevcutsa [`Row`](../../row/) nesnesini döndürür, aksi takdirde null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Bazı verileri doldurun
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Satırın var olup olmadığını kontrol et ve satır nesnesini al
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Var olmayan satırı kontrol et
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


