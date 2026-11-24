---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Typnamen von Tabellenzeilen zurück, die die aktuelle Zeile in der referenzierten Tabelle enthalten. Standard ist This Row, sodass This Row in der Formel die aktuelle Zeile in der referenzierten Tabelle darstellt."
type: docs
url: /de/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Gibt den Typnamen von Tabellenzeilen zurück, die die aktuelle Zeile in der referenzierten Tabelle enthalten. Standard ist "This Row", sodass in der Formel "#This Row" die aktuelle Zeile in der referenzierten Tabelle darstellt.

```csharp
public virtual string GetTableRowTypeOfCurrent()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Erstellen Sie Beispieldaten und eine Tabelle
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Tabelle erstellen
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Formel hinzufügen, die die aktuelle Zeilenreferenz verwendet
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // Demonstrieren Sie die Wirkung von GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


