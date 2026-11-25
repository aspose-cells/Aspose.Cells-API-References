---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Restituisce il testo dell'etichetta Totale nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

Restituisce il testo dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati.

```csharp
public override string GetTextOfTotal()
```

### Valore di ritorno

Il testo dell'etichetta "Totale"

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il contesto
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
                // Imposta testo personalizzato per l'etichetta "Totale"
                settings.SetTextOfTotal("Custom Total");

                // Ottieni il testo dell'etichetta "Totale"
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


