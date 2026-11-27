---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Returnerar en array som innehåller namn på teckensnittssubstitut som ska användas om originalteckensnittet inte finns"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Returnerar en array som innehåller teckensnittsersättningsnamn som ska användas om originalteckensnittet inte finns.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Returvärde

En array som innehåller namn på teckensnittssubstitut som ska användas om originalteckensnittet inte finns.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Skapa individuella teckensnittskonfigurationer
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Ange teckensnittssubstitut för "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Hämta teckensnittssubstitut för "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Skapa en arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ange stil med originalteckensnitt
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Spara arbetsboken
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


