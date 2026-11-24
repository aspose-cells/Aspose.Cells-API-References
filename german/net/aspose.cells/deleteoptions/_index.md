---
title: "Klasse DeleteOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DeleteOptions Klasse. Stellt die Einstellung zum Löschen von Zeilen/Spalten dar."
type: docs
url: /de/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Stellt die Einstellung zum Löschen von Zeilen/Spalten dar.

```csharp
public class DeleteOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Liest/setzt den Monitor zur Verfolgung von Änderungen, die durch das Löschen verursacht werden. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Anzeige der Originaldaten
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // DeleteOptions erstellen
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Lösche die zweite Zeile (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Anzeige der Daten nach dem Löschen
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


