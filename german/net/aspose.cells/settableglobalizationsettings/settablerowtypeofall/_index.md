---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Legt den Typnamen von Tabellenzeilen fest, die aus allen Zeilen in der referenzierten Tabelle bestehen"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

Legt den Typnamen von Tabellenzeilen fest, die alle Zeilen der referenzierten Tabelle enthalten.

```csharp
public void SetTableRowTypeOfAll(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für eine Tabelle erstellen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Eine Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie SetTableRowTypeOfAll mit benutzerdefiniertem Namen auf
                settings.SetTableRowTypeOfAll("CompleteTable");

                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = settings;

                // Überprüfen Sie die Einstellung, indem Sie den Wert zurückholen
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // Fügen Sie eine Formel hinzu, die alle Zeilen mit dem benutzerdefinierten Namen referenziert
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // Formeln berechnen
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


