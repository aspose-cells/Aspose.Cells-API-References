---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportRangeToJsonOptions-Eigenschaft. Gibt an, ob leere Zellen als null exportiert werden"
type: docs
url: /de/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Gibt an, ob leere Zellen als null exportiert werden.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // Lassen Sie B2 absichtlich leer
            
            // Exportoptionen erstellen und das Exportieren leerer Zellen aktivieren
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // Exportiere den Bereich nach JSON
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### Siehe auch

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


