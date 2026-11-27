---
title: "Row.FirstDataCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar den första icke-tomma cellen i raden"
type: docs
url: /sv/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Hämtar den första icke‑tomma cellen i raden.

```csharp
public Cell FirstDataCell { get; }
```

### Exempel

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
            
            // Placera värden i olika celler
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Hämta den första datacellen i rad 1 (index 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Hämta den första datacellen i rad 2 (index 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


