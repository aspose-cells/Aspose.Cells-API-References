---
title: "SettablePivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta Column Labels nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

Restituisce il testo dell'etichetta "Column Labels" nella PivotTable.

```csharp
public override string GetTextOfColumnLabels()
```

### Valore di ritorno

Il testo delle etichette di colonna

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il contesto
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ottieni il testo predefinito delle etichette di colonna
                string columnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default text of Column Labels: {columnLabelsText}");

                // Imposta testo personalizzato per le etichette di colonna
                settings.SetTextOfColumnLabels("Custom Column Headers");

                // Ottieni il testo aggiornato delle etichette di colonna
                string updatedColumnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Updated text of Column Labels: {updatedColumnLabelsText}");

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfColumnLabelsDemo.xlsx");
                Console.WriteLine("GetTextOfColumnLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


