---
title: "Style.GetTwoColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Hämta tvåfärgsgradientinställningen"
type: docs
url: /sv/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Hämta den tvåfärgade gradientinställningen.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | Color& | En gradientfärg. |
| color2 | Color& | Två gradientfärger. |
| gradientStyleType | GradientStyleType& | Gradientskuggningsstil. |
| variant | Int32& | Gradientvarianten. |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället Style.GetTwoColorGradientSetting()‑metoden. Den här egenskapen kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil och ställ in tvåfärgsgradient
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Förbered variabler för att hämta gradientinställningar
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Anropa GetTwoColorGradient‑metoden
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Visa de hämtade gradientinställningarna
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Spara arbetsboken
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


