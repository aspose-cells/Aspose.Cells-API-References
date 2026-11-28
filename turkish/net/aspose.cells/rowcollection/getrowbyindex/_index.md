---
title: "RowCollection.GetRowByIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RowCollection yöntemi. Listedeki konuma göre satır nesnesini alır."
type: docs
url: /tr/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Listedeki konuma göre satır nesnesini alır.

```csharp
public Row GetRowByIndex(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Konum. |

### Dönüş Değeri

Verilen konumdaki Row nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Satırı indeksle al (0 tabanlı)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


