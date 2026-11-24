---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt an, ob leere Zellen als null exportiert werden"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Gibt an, ob leere Zellen als null exportiert werden.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten mit einigen leeren Zellen füllen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // JsonSaveOptions mit ExportEmptyCells auf false erstellen
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Als JSON speichern – leere Zellen werden übersprungen
            workbook.Save("output_skip_empty.json", options);

            // ExportEmptyCells auf true ändern
            options.ExportEmptyCells = true;

            // Erneut speichern – leere Zellen werden eingeschlossen
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


