---
title: "Range.IsIntersect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Anger om området skär varandra"
type: docs
url: /sv/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Anger om området intersecteras.

```csharp
public bool IsIntersect(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Området. |

### Returvärde

Om området skär varandra.

### Anmärkningar

Om de två områdena inte är i samma kalkylblad, returnera falskt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två områden för att testa intersektion.
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // Kontrollera om range1 intersectar med range2 (bör intersecta).
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // Kontrollera om range1 intersectar med range3 (bör inte intersecta).
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Fyll områdena med olika färger för att visualisera dem.
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


