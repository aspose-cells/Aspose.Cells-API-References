---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs‑Methode. Gibt ein Array zurück, das Schriftart‑Ersetzungsnamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist."
type: docs
url: /de/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Rückgabewert

Ein Array, das Schriftart‑Ersetzungsnamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Initialisieren Sie FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Rufen Sie GetFontSubstitutes mit einem Schriftartnamen auf
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Ergebnisse anzeigen
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

                // Demonstrieren Sie das Festlegen von Ersetzungen und das Abrufen dieser.
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Rufen Sie die Ersetzungen erneut ab, um zu überprüfen.
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

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


