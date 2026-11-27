---
title: "JsonSaveOptions.Indent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger indraget"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Indikerar indraget.

```csharp
public string Indent { get; set; }
```

### Anmärkningar

Om indraget är null eller tomt, formateras inte den exporterade JSON‑filen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Konfigurera JSON‑sparalternativ med indrag
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Spara med indragen JSON‑utdata
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


