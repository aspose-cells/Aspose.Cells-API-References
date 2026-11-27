---
title: "JsonSaveOptions.ExportArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Hämtar eller anger exportområdet"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

Hämtar eller anger exportintervallet.

```csharp
public CellArea ExportArea { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Konfigurera JSON-sparalternativ med ExportArea
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Spara med angivet exportområde (A1:B3)
            workbook.Save("JsonExportAreaDemo.json", saveOptions);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


