---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metod. Teckensnittssubstitutnamn för angivet originalteckensnitt"
type: docs
url: /sv/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Namn på teckensnittssubstitut för angivet originalteckensnitt.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Originalt teckensnittnamn som kanske inte är tillgängligt
            string originalFontName = "Arial";
            
            // Substitutnamn för teckensnitt att använda när originalet inte är tillgängligt
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Anropa SetFontSubstitutes-metoden för att konfigurera teckensnittssubstitutioner
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Verifiera ersättningarna genom att hämta dem
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Applicera teckensnittet på en cell för att demonstrera ersättning
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


