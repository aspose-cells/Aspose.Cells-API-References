---
title: "Range.ToJson"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Converte l'intervallo in valore JSON"
type: docs
url: /it/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Converti l'intervallo in valore JSON.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | JsonSaveOptions | Le opzioni di conversione |

### Esempi

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
            
            // Dati di esempio
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

### Vedi anche

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


