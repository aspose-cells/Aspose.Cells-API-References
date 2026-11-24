---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Legt den Typnamen von Tabellenzeilen fest, die aus der aktuellen Zeile in der referenzierten Tabelle bestehen"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Legt den Typnamen von Tabellenzeilen fest, die die aktuelle Zeile in der referenzierten Tabelle enthalten.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Benutzerdefinierten Namen für den aktuellen Zeilentyp festlegen
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = settings;

                // Überprüfen Sie die Einstellung, indem Sie den Wert zurückholen
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


