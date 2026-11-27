---
title: "UnionRange.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑metod. Hämtar enumeratorn för celler i detta Range"
type: docs
url: /sv/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Hämtar enumeratorn för celler i detta område.

```csharp
public IEnumerator GetEnumerator()
```

### Returvärde

Cellernas enumerator

### Anmärkningar

När du traverserar element med den returnerade Enumeratorn bör cellsamlingen inte modifieras (såsom operationer som skapar nya Cell/Row eller tar bort befintliga Cell/Row). Annars kan enumeratorn misslyckas med att traversera alla celler korrekt (vissa element kan traverseras flera gånger eller hoppas över).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa det första området (A1:B2) och fyll det med data
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Skapa det andra området (C1:D2) och fyll det med data
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Bygg en UnionRange från det första området
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Lägg till det andra området i unionen
                unionRange = unionRange.Union("C1:D2");

                // Hämta enumeratorn och iterera genom alla celler i unionen
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Spara arbetsboken (valfritt, bara för att visa att data kvarstår)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


