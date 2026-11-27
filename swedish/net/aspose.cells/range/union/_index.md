---
title: "Range.Union"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Returnerar unionen av två områden"
type: docs
url: /sv/net/aspose.cells/range/union/
---
## Range.Union method

Returnerar unionen av två områden.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Området |

### Returvärde

Föreningen av två områden.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Range.UnionRanges()-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två områden för att demonstrera Union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Fyll i lite data i områdena
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Anropa Union-metoden (obs: detta är den föråldrade versionen)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Visa adresser för alla intervall i unionen
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


