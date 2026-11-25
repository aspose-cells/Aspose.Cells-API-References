---
title: "SettablePivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo del tipo PivotFieldSubtotalType nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofsubtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method

Ottiene il testo del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella PivotTable.

```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Il [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valore di ritorno

Il testo del tipo specificato

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Chiama GetTextOfSubTotal con valori diversi di PivotFieldSubtotalType
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);

                // Visualizza i risultati
                Console.WriteLine($"Sum subtotal text: {sumText}");
                Console.WriteLine($"Average subtotal text: {avgText}");
                Console.WriteLine($"Count subtotal text: {countText}");

                // Imposta testo personalizzato per i subtotali
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");

                // Verifica le modifiche
                Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
                Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


