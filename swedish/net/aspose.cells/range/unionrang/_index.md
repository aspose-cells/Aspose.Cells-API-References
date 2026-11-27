---
title: "Range.UnionRang"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Returnerar föreningsresultatet av två områden"
type: docs
url: /sv/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Returnerar unionsresultatet av två områden.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Området |

### Returvärde

Föreningen av två områden.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Range.UnionRanges()-metoden. Denna metod kommer att tas bort 12 månader senare från och med maj 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två områden för att demonstrera UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Ange några värden i områdena för visualisering
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Anropa UnionRang-metoden för att kombinera de två områdena
                Range[] unionResult = range1.UnionRang(range2);

                // Visa information om unionresultatet
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Markera unionområdena med en ram för visualisering
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


