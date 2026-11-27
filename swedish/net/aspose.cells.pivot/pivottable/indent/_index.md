---
title: "PivotTable.Indent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Anger indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form.

```csharp
public int Indent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ställ in indenteringsegenskapen
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Spara arbetsboken
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


