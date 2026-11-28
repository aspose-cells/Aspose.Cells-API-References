---
title: "Row.GetCellByIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row yöntemi. Bu satırın hücre koleksiyonundaki belirli indekse göre hücreyi al"
type: docs
url: /tr/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Bu satırın hücre koleksiyonundaki belirli indeksle hücreyi al.

```csharp
public Cell GetCellByIndex(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Bu satırın hücre koleksiyonundaki hücrenin indeks(konumu). |

### Dönüş Değeri

Verilen konumdaki Cell nesnesi.

### Açıklamalar

Tüm hücreleri sırasıyla, değişiklik yapmadan dolaşmak için [`GetEnumerator`](../getenumerator/) kullanmak, bu yöntemi tek tek hücre almak için kullanmaktan daha iyi performans sağlar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk satırdaki hücrelere veri ekle
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // İlk satırı al.
            Row row = worksheet.Cells.Rows[0];

            // Int32 parametresiyle GetCellByIndex'i göster
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


