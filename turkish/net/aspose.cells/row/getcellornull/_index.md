---
title: "Row.GetCellOrNull"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row yöntemi. Belirli indekste hücreyi veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Belirli indeksteki hücreyi veya null değerini alır.

```csharp
public Cell GetCellOrNull(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi |

### Dönüş Değeri

Hücre mevcutsa hücre nesnesini döndürür. Hücre nesnesi yoksa null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Örnek veri ekleyin.
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // İlk satırı al
            Row row = ws.Cells.Rows[0];

            // Int32 parametresiyle GetCellOrNull'u göster
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


