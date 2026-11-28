---
title: "WorksheetCollection.CreateRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Aralığın adresinden bir Range nesnesi oluşturur"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Bir [`Range`](../../range/) nesnesini aralığın adresinden oluşturur.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| address | String | Aralığın adresi. |
| sheetIndex | Int32 | Sayfa indeksi. |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biraz örnek veri doldurun
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Dize adresi ve sayfa indeksi kullanarak aralık oluştur
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Aralık kullanımını göster
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


