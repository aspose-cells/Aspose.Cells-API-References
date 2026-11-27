---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metod. Anger texten för typen PivotFieldSubtotalType i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Anger texten för typen [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) i pivottabellen.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| text | String | Texten för given typ |

### Exempel

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
            // Skapa en ny arbetsbok (endast för demonstrationsändamål)
            Workbook workbook = new Workbook();

            // Instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ange anpassad text för Sum-subtotalen
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Verifiera ändringen
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Ange anpassad text för Average-subtotalen
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Verifiera ändringen
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Spara arbetsboken (inga pivottabellsändringar i den här demonstrationen)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


