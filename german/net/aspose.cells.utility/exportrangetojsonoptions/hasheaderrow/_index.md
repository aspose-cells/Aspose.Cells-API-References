---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportRangeToJsonOptions Eigenschaft. Gibt an, ob der Bereich eine Kopfzeile enthält"
type: docs
url: /de/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Gibt an, ob der Bereich eine Kopfzeilenzeile enthält.

```csharp
public bool HasHeaderRow { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Kopfzeilen füllen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Bereich zum Exportieren erstellen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // ExportRangeToJsonOptions-Instanz erstellen
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Aktuellen HasHeaderRow-Wert anzeigen (Standard ist false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // HasHeaderRow auf true setzen
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportieren nach JSON mit Kopfzeilen
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // HasHeaderRow auf false setzen
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportieren nach JSON ohne Kopfzeilen
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


