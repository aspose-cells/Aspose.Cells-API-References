---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metoden. Returnerar en array som innehåller namn på teckensnittssubstitut som ska användas om originalteckensnittet inte finns"
type: docs
url: /sv/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Returnerar en array som innehåller namn på teckensnittssubstitut som ska användas om originalteckensnittet saknas.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Initiera FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Anropa GetFontSubstitutes med ett teckensnittsnamn
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Visa resultaten
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // Visa hur man ställer in substitut och hämtar dem
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Hämta substituten igen för att verifiera
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


