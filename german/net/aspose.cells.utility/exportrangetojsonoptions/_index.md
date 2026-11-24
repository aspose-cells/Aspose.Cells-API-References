---
title: "Klasse ExportRangeToJsonOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Utility.ExportRangeToJsonOptions Klasse. Gibt die Optionen an, die beim Exportieren eines Bereichs nach JSON verwendet werden"
type: docs
url: /de/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Gibt die Optionen an, die beim Exportieren eines Bereichs nach JSON verwendet werden.

```csharp
public class ExportRangeToJsonOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exportiert den Zeichenkettenwert der Zellen nach JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Gibt an, ob leere Zellen als null exportiert werden. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Gibt an, ob der Bereich eine Kopfzeilenzeile enthält. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Gibt die Einrückung an. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Erstelle Exportoptionen
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Exportiere Bereich nach JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Gib das JSON aus
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // In Datei speichern (optional)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


