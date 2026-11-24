---
title: "SettablePivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text des Typs PivotFieldSubtotalType in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofsubtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method

Gibt den Text des Typs [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) in der PivotTable zurück.

```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Der [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Rückgabewert

Der Text des angegebenen Typs

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Rufen Sie GetTextOfSubTotal mit verschiedenen PivotFieldSubtotalType-Werten auf
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);

                // Ergebnisse anzeigen
                Console.WriteLine($"Sum subtotal text: {sumText}");
                Console.WriteLine($"Average subtotal text: {avgText}");
                Console.WriteLine($"Count subtotal text: {countText}");

                // Legen Sie benutzerdefinierten Text für Zwischensummen fest
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");

                // Änderungen überprüfen
                Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
                Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


