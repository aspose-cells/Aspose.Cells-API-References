---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Legt den Typnamen von Tabellenzeilen fest, die aus dem Datenbereich der referenzierten Tabelle bestehen"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Legt den Typnamen von Tabellenzeilen fest, die den Datenbereich der referenzierten Tabelle enthalten.

```csharp
public void SetTableRowTypeOfData(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Tabelle erstellen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Benutzerdefinierten Namen für Datenzeilen in der Tabelle festlegen
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


