---
title: "DeleteBlankOptions.EndIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions property. Anger slutrad/kolumnindexet (inklusive) för det område som ska kontrolleras och radera tomma rader/kolumner. Standardvärdet är 1 och 1 betyder det maximala området för alla objektceller‑ritningar … som måste kontrolleras"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Specificerar slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och där tomma rader/kolumner tas bort. Standardvärdet är -1 och -1 betyder det maximala intervallet för alla objekt (celler, ritningar, ...) som måste kontrolleras.

```csharp
public int EndIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Fyll i några celler med värden
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Skapa raderingsalternativ med specifikt område
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Radera tomma kolumner inom angivet område
            cells.DeleteBlankColumns(dbo);

            // Skriv ut resultat för att demonstrera effekten av EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Se även

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


