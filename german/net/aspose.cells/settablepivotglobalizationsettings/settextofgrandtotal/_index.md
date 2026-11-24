---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Legt den Text der \"Grand Total\"-Beschriftung in der PivotTable fest"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Setzt den Text des "Grand Total"-Labels in der PivotTable.

```csharp
public void SetTextOfGrandTotal(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | benutzerdefinierter Text |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe (nur Kontext)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Legen Sie einen benutzerdefinierten Text für die "Grand Total"-Beschriftung fest
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Rufen Sie den aktualisierten Beschriftungstext ab, um die Änderung zu überprüfen
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Speichern Sie die Arbeitsmappe nur, um zu demonstrieren, dass der Code ohne Fehler läuft
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

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


