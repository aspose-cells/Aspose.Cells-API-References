---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta Grand Total nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Restituisce il testo dell'etichetta "Grand Total" nella PivotTable.

```csharp
public override string GetTextOfGrandTotal()
```

### Valore di ritorno

Il testo dell'etichetta "Grand Total"

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook (solo per contesto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Modifica il testo predefinito "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Recupera il testo corrente "Grand Total"
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Salva la cartella di lavoro (non viene creata alcuna pivot table, ma il file viene salvato per dimostrare l'esecuzione)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


