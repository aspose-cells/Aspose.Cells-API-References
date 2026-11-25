---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta Column Labels nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Restituisce il testo dell'etichetta "Column Labels" nella PivotTable.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo delle etichette di colonna |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook (solo per contesto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Crea un'istanza di SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // Imposta testo personalizzato per l'etichetta "Column Labels"
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Recupera il testo corrente per verificare la modifica
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Salva il workbook (non è necessaria alcuna pivot table per questa demo)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


