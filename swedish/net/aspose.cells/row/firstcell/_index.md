---
title: "Row.FirstCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row egenskap. Hämtar det första cellobjektet i raden"
type: docs
url: /sv/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Hämtar det första cellobjektet i raden.

```csharp
public Cell FirstCell { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till data i cellerna i den första raden
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Hämta den första raden
            Row row = worksheet.Cells.Rows[0];
            
            // Demonstrera FirstCell-egenskapen
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Ändra den första cellen
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Spara arbetsboken
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


