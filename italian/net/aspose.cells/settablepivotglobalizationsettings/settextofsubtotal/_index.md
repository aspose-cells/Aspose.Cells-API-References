---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Imposta il testo del tipo PivotFieldSubtotalType nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Imposta il testo del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella PivotTable.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Il [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| testo | String | Il testo del tipo specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook (solo a scopo dimostrativo)
            Workbook workbook = new Workbook();

            // Istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Imposta testo personalizzato per il subtotale Sum
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Verifica la modifica
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Imposta testo personalizzato per il subtotale Average
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Verifica la modifica
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Salva il workbook (nessuna modifica alla pivot table in questa demo)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


