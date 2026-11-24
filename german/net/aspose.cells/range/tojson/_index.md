---
title: "Range.ToJson"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Konvertiert den Bereich in einen JSON-Wert"
type: docs
url: /de/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Konvertiert den Bereich in einen JSON-Wert.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | JsonSaveOptions | Die Optionen der Konvertierung |

### Beispiele

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
            
            // Beispieldaten
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

### Siehe auch

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


