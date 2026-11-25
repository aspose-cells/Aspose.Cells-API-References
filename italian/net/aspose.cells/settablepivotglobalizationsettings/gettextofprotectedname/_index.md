---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo per il nome protetto specificato"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Restituisce il testo per il nome protetto specificato.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectedName | String | Il nome protetto nella PivotTable. |

### Valore di ritorno

I nomi protetti locali della PivotTable.

### Osservazioni

In Ms Excel, alcuni nomi non possono essere usati come nome dei PivotField nella PivotTable. Sono diversi a seconda della regione; l'utente può specificarli esplicitamente in base alla regione utilizzata.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il contesto
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Imposta un testo personalizzato per un nome protetto
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Ottieni il testo del nome protetto
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


