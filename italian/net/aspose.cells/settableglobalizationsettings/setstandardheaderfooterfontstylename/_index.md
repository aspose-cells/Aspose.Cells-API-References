---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localfontStyleName | String | Nome dello stile di carattere locale per Intestazione/Piè di pagina. |
| standardName | String | Nome della funzione Standard (locale en-US). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea le opzioni di impostazione pagina per il foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta un'intestazione con del testo
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Crea un'istanza delle impostazioni di globalizzazione
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Chiama il metodo SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Applica le impostazioni di globalizzazione al workbook
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // L'effetto sarà visibile quando il documento viene renderizzato o stampato
                // Lo stile di carattere "Arial" nelle intestazioni/piè di pagina sarà trattato come "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


