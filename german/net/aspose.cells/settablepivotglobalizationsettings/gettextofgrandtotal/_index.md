---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text der \"Grand Total\"‑Beschriftung in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Ermittelt den Text der Beschriftung "Grand Total" in der PivotTable.

```csharp
public override string GetTextOfGrandTotal()
```

### Rückgabewert

Der Text der "Grand Total"‑Beschriftung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe (nur zum Kontext)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ändern Sie den Standardtext der "Grand Total"‑Beschriftung
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Rufen Sie den aktuellen Text der "Grand Total"‑Beschriftung ab
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Speichern Sie die Arbeitsmappe (es wird keine PivotTable erstellt, aber die Datei wird gespeichert, um die Ausführung zu beweisen)
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

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


