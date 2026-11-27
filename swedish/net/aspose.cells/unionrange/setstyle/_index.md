---
title: "UnionRange.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-metod. Ställer in stil för området"
type: docs
url: /sv/net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Ställer in stilen för området.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Style-objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några exempeldata i området A1:B2
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue("Total");
            worksheet.Cells["B2"].PutValue(456);

            // Skapa ett UnionRange som täcker cellerna A1:B2
            UnionRange unionRange = worksheet.Cells
                .CreateRange("A1:B2")
                .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Skapa en Style-instans och ange någon formatering
                Style style = new Style();
                style.BackgroundColor = Color.LightYellow;
                style.ForegroundColor = Color.DarkBlue;
                style.HorizontalAlignment = TextAlignmentType.Center;
                style.VerticalAlignment = TextAlignmentType.Center;
                style.IsTextWrapped = true;

                // Applicera stilen på unionområdet
                unionRange.SetStyle(style);

                Console.WriteLine("SetStyle executed successfully on the UnionRange.");

                // Spara arbetsboken för att visualisera resultatet
                workbook.Save("UnionRangeSetStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetStyle: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


