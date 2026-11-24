---
title: "SettableGlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den Typnamen von Tabellenzeilen zurück, die aus der Gesamtsumme‑Zeile der referenzierten Tabelle bestehen"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/
---
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method

Gibt den Typnamen von Tabellenzeilen zurück, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten.

```csharp
public override string GetTableRowTypeOfTotals()
```

### Rückgabewert

der Typname von Tabellenzeilen

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");

            // Ein ListObject (Tabelle) erstellen
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfTotals("CustomTotals");

            try
            {
                // Den Tabellereihen‑Typ für Summen abrufen
                string rowType = settings.GetTableRowTypeOfTotals();
                Console.WriteLine($"Table row type for totals: {rowType}");

                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = settings;

                // Überprüfen Sie die Auswirkung in einer Formel
                worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
                Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


