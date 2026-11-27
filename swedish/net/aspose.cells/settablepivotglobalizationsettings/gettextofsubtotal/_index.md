---
title: "SettablePivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för typen PivotFieldSubtotalType i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofsubtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method

Hämtar texten för typen [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) i pivottabellen.

```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Returvärde

Texten för given typ

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Anropa GetTextOfSubTotal med olika PivotFieldSubtotalType‑värden
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);

                // Visa resultaten
                Console.WriteLine($"Sum subtotal text: {sumText}");
                Console.WriteLine($"Average subtotal text: {avgText}");
                Console.WriteLine($"Count subtotal text: {countText}");

                // Ange anpassad text för delsummor
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");

                // Verifiera ändringarna
                Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
                Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


