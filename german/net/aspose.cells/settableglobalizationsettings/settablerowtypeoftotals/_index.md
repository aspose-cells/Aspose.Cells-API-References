---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt den Typnamen von Tabellenzeilen fest, die aus der Gesamtsumme‑Zeile der referenzierten Tabelle bestehen"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

Legt den Typnamen von Tabellenzeilen fest, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten.

```csharp
public void SetTableRowTypeOfTotals(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | der Typname von Tabellenzeilen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Tabelle erstellen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie SetTableRowTypeOfTotals mit benutzerdefiniertem Namen auf
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


