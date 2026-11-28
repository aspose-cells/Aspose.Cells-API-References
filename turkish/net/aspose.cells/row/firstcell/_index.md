---
title: "Row.FirstCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırdaki ilk hücre nesnesini alır."
type: docs
url: /tr/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Satırdaki ilk hücre nesnesini alır.

```csharp
public Cell FirstCell { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk satırdaki hücrelere veri ekle
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // İlk satırı al
            Row row = worksheet.Cells.Rows[0];
            
            // FirstCell özelliğini göster
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // İlk hücreyi değiştir
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


