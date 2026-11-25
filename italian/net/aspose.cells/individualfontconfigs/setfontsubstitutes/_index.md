---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Imposta i nomi dei sostituti dei font per un dato nome di font originale"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Imposta i nomi dei caratteri sostitutivi per un dato nome di carattere originale.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| originalFontName | String | Nome del font originale. |
| substituteFontNames | String[] | Elenco dei nomi dei font sostitutivi da utilizzare se il font originale non è presente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un'istanza di IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Nome del font originale e i suoi sostituti
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Chiama SetFontSubstitutes con i parametri specificati
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Crea una cartella di lavoro per dimostrare l'effetto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Imposta lo stile con il font originale
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


