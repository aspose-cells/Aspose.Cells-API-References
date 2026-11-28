---
title: "Row.LastCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırdaki son hücre nesnesini alır"
type: docs
url: /tr/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Satırdaki son hücre nesnesini alır.

```csharp
public Cell LastCell { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // İlk satırı al
            Row row = worksheet.Cells.Rows[0];

            // Satırdaki son hücreye eriş
            Cell lastCell = row.LastCell;
            
            // Son hücrenin değerini çıktı olarak ver
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


