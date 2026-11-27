---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om tomma celler exporteras som null"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Anger om tomma celler ska exporteras som null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll data med några tomma celler
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // Skapa JsonSaveOptions med ExportEmptyCells satt till false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Spara till JSON - tomma celler kommer att hoppas över
            workbook.Save("output_skip_empty.json", options);

            // Ändra ExportEmptyCells till true
            options.ExportEmptyCells = true;

            // Spara igen - tomma celler kommer att inkluderas
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


