---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Legt den Text der Beschriftung \"Multiple Items\" in der PivotTable fest"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

Setzt den Text des "(Multiple Items)"-Labels in der PivotTable.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu (optional, nur zum Kontext)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Erstelle eine Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Benutzerdefinierten Text für die "(Multiple Items)"-Beschriftung in einer PivotTable festlegen
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // Rufen Sie den aktualisierten Text ab und zeigen Sie ihn an
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (Optional) Speichern Sie die Arbeitsmappe – eine PivotTable ist für diese Demo nicht erforderlich
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


