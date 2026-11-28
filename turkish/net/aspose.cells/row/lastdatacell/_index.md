---
title: "Row.LastDataCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırdaki son boş olmayan hücreyi alır"
type: docs
url: /tr/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Satırdaki son boş olmayan hücreyi alır.

```csharp
public Cell LastDataCell { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Hücrelere veri koy
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // İlk satırdaki son veri hücresini al
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


