---
title: "Range.ToJson"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Konvertera området till JSON-värde"
type: docs
url: /sv/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Konvertera området till JSON‑värde.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | JsonSaveOptions | Alternativen för konvertering |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToJsonWithJsonSaveOptionsDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            
            // Exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);

            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


