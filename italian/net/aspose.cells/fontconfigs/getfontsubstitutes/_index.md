---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Restituisce un array contenente i nomi dei sostituti dei font da utilizzare se il font originale non è presente"
type: docs
url: /it/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Restituisce un array contenente i nomi delle sostituzioni di carattere da utilizzare se il carattere originale non è presente.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Valore di ritorno

Un array contenente i nomi dei sostituti dei font da utilizzare se il font originale non è presentato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Inizializza FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Chiama GetFontSubstitutes con un nome di font
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Visualizza i risultati
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

                // Dimostra l'impostazione dei sostituti e il loro recupero
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Ottieni nuovamente i sostituti per verificare
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

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


