---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Nomi dei font sostitutivi per il nome del font originale fornito"
type: docs
url: /it/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Nomi delle sostituzioni di carattere per il nome del carattere originale fornito.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nome del font originale che potrebbe non essere disponibile
            string originalFontName = "Arial";
            
            // Nomi dei font sostitutivi da usare quando l'originale non è disponibile
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Chiama il metodo SetFontSubstitutes per configurare le sostituzioni dei font
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Verifica le sostituzioni recuperandole
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Applica il font a una cella per dimostrare la sostituzione
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


