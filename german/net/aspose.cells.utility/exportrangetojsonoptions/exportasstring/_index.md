---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportRangeToJsonOptions Eigenschaft. Exportiert den Zeichenkettenwert der Zellen nach JSON"
type: docs
url: /de/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Exportiert den Zeichenkettenwert der Zellen nach JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zellen mit verschiedenen Datentypen füllen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // ExportRangeToJsonOptions-Instanz erstellen
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Aktuellen ExportAsString-Wert anzeigen
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Export ohne ExportAsString (Standardverhalten)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // Setze ExportAsString auf true
            options.ExportAsString = true;

            // Export mit ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Speichere die Arbeitsmappe
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


