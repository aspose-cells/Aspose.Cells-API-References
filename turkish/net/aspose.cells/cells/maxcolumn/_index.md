---
title: "Cells.MaxColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Koleksiyonda örneklenmiş hücrelerin maksimum sütun indeksi, tüm sütun için stil tanımlı olduğu ancak hiçbir hücrenin örneklenmediği sütunu içermez."
type: docs
url: /tr/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Koleksiyonda oluşturulmuş hücrelerin maksimum sütun indeksi (tüm sütun için stil tanımlı ancak içinde hücre oluşturulmamış sütunu içermez).

```csharp
public int MaxColumn { get; }
```

### Açıklamalar

Hiç hücre örneklenmemişse -1 döndürün.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Veri içeren maksimum sütun indeksini alın.
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Maksimum sütundan sonraki bir sonraki sütuna veri ekleyin.
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Yeni maksimum sütunu doğrulayın.
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Kopyalamayı göstermek için başka bir çalışma sayfası oluşturun.
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Tüm sütunları kaynaktan hedefe kopyalayın.
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


