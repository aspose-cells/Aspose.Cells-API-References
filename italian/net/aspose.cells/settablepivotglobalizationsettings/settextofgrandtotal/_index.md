---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Imposta il testo dell'etichetta Grand Total nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Imposta il testo dell'etichetta "Grand Total" nella PivotTable.

```csharp
public void SetTextOfGrandTotal(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | testo personalizzato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro (solo contesto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Imposta un testo personalizzato per l'etichetta "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Recupera il testo aggiornato dell'etichetta per verificare la modifica
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Salva la cartella di lavoro solo per dimostrare che il codice viene eseguito senza errori
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


