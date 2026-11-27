---
title: "Range.UnionRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Returnerar föreningsresultatet av två områden"
type: docs
url: /sv/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Returnerar unionsresultatet av två områden.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | Range[] | Området |

### Returvärde

Föreningen av två områden.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata i celler
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Skapa ranges för union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Anropa UnionRanges med Range[]-parameter
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Applicera stil för att visa den förenade range
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


