---
title: "JsonSaveOptions.ExportAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Exporterar cellernas strängvärde till json"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Exporterar cellernas strängvärde till JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Skapa exempeldata med numeriska värden
            cells["A1"].PutValue("Age");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue(30);
            cells["B2"].PutValue(95.5);

            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
            Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


