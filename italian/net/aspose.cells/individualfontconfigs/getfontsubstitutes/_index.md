---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Restituisce un array contenente i nomi dei sostituti dei caratteri da utilizzare se il carattere originale non è presente"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Restituisce un array contenente i nomi dei caratteri sostitutivi da utilizzare se il carattere originale non è presente.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
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

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Crea configurazioni di font individuali
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Imposta i sostituti dei caratteri per "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Ottieni i sostituti dei caratteri per "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Crea una cartella di lavoro per dimostrare l'effetto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Imposta lo stile con il font originale
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Salva la cartella di lavoro
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

### Vedi anche

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


