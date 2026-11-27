---
title: "Klass ExportRangeToJsonOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Utility.ExportRangeToJsonOptions-klass. Anger alternativen för att exportera område till json"
type: docs
url: /sv/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Anger alternativen för att exportera ett område till JSON.

```csharp
public class ExportRangeToJsonOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exporterar cellernas strängvärde till JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Anger om tomma celler ska exporteras som null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Anger om intervallet innehåller en rubrikrad. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indikerar indraget. |

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa exportalternativ
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Exportera område till JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Skriv ut JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Spara till fil (valfritt)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


