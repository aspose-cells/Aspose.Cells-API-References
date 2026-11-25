---
title: "SettablePivotGlobalizationSettings.SetTextOfEmptyData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Imposta il testo dell'etichetta vuota nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Imposta il testo dell'etichetta "(blank)" nella PivotTable.

```csharp
public void SetTextOfEmptyData(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo dei dati vuoti |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio (opzionale, solo per contesto)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Imposta testo personalizzato per le celle di dati vuoti in una PivotTable
                settings.SetTextOfEmptyData("(no data)");

                // Verifica la modifica
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Custom text for empty data: {emptyDataText}");

                // (Opzionale) Salva la cartella di lavoro – anche se non abbiamo creato una PivotTable,
                // ciò dimostra che la cartella di lavoro può ancora essere salvata dopo la manipolazione delle impostazioni.
                workbook.Save("SetTextOfEmptyDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


