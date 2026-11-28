---
title: "Cells.CheckColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütun indeksinde Column öğesini veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Belirtilen sütun indeksinde [`Column`](../../column/) öğesini alır veya null döner.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi. |

### Dönüş Değeri

Column nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sütun 1'de (B3) bir değer ayarla
            cells["B3"].PutValue("Sample Data");
            
            // Sütun 4'ü kontrol et (E sütunu)
            Column column = cells.CheckColumn(4);
            
            // Sütun özelliklerini çıktı al
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


