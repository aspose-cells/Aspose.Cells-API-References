---
title: "SettablePivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text der \"Multiple Items\"‑Beschriftung in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Ermittelt den Text der Beschriftung "(Multiple Items)" in der PivotTable.

```csharp
public override string GetTextOfMultipleItems()
```

### Rückgabewert

Der Text der "(Multiple Items)"‑Beschriftung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten zum Kontext hinzufügen
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
                // Den Standardtext für mehrere Elemente abrufen
                string multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {multipleItemsText}");

                // Legen Sie einen benutzerdefinierten Text für mehrere Elemente fest
                settings.SetTextOfMultipleItems("(Multiple Items Custom)");
                multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Updated text for multiple items: {multipleItemsText}");

                // Speichere die Arbeitsmappe
                workbook.Save("GetTextOfMultipleItemsDemo.xlsx");
                Console.WriteLine("GetTextOfMultipleItems method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


