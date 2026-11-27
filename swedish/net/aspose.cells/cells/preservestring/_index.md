---
title: "Cells.PreserveString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. Standard är falskt."
type: docs
url: /sv/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Hämtar eller anger ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. Standard är falskt.

```csharp
public bool PreserveString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in PreserveString-egenskapen till true
            cells.PreserveString = true;

            // Lägg till strängvärden i celler
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Åtkomst till värdena (de kommer att bevaras som strängar)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Spara arbetsboken
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera bevarandet
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Skriv ut de bevarade värdena
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Demonstrera jämförelse av PreserveString‑egenskapen
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


