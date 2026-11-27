---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Anger namn på teckensnittssubstitut för ett givet originalteckensnitt"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Ställer in teckensnittsersättningsnamn för ett givet originalteckensnittsnamn.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| originalFontName | String | Originalt teckensnittnamn. |
| substituteFontNames | String[] | Lista över teckensnittssubstitutnamn som ska användas om originalteckensnittet inte finns. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en instans av IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Originalt teckensnittsnamn och dess substitut
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Anropa SetFontSubstitutes med de angivna parametrarna
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Skapa en arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ange stil med originalteckensnitt
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Spara arbetsboken
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


