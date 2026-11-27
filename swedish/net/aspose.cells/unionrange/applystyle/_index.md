---
title: "UnionRange.ApplyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-metod. Tillämpar format för ett helt intervall"
type: docs
url: /sv/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Tillämpar format för ett helt område.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Anmärkningar

Varje cell i detta range kommer att innehålla ett [`Style`](../../style/)‑objekt. Så detta är en minneskrävande metod. Använd den försiktigt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett UnionRange som täcker cellerna A1 till B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Skapa en stil med specifik formatering
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Skapa en StyleFlag för att ange vilka egenskaper som ska tillämpas
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Anropa ApplyStyle med stil- och flaggparametrarna
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


