---
title: "Row.FirstDataCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırdaki ilk boş olmayan hücreyi alır"
type: docs
url: /tr/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Satırdaki ilk boş olmayan hücreyi alır.

```csharp
public Cell FirstDataCell { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Farklı hücrelere değerler koy
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Satır 1'deki (indeks 0) ilk veri hücresini al
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Satır 2'deki (indeks 1) ilk veri hücresini al
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


