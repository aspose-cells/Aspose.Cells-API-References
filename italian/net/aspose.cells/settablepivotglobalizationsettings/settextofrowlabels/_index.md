---
title: "SettablePivotGlobalizationSettings.SetTextOfRowLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Imposta il testo dell'etichetta Row Labels nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

Imposta il testo dell'etichetta "Row Labels" nella PivotTable.

```csharp
public void SetTextOfRowLabels(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo delle etichette di riga |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il contesto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            SettablePivotGlobalizationSettings pivotSettings = new SettablePivotGlobalizationSettings();
            globalizationSettings.PivotSettings = pivotSettings;

            try
            {
                // Imposta testo personalizzato per "Etichette riga"
                pivotSettings.SetTextOfRowLabels("Custom Row Labels");

                // Verifica la modifica
                string rowLabelsText = pivotSettings.GetTextOfRowLabels();
                Console.WriteLine($"Row Labels text after change: {rowLabelsText}");

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Salva la cartella di lavoro
                workbook.Save("SetTextOfRowLabelsDemo.xlsx");
                Console.WriteLine("SetTextOfRowLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


