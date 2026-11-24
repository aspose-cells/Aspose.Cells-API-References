---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLayoutOptions-Eigenschaft. Verarbeitet Arrays als Tabelle"
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Verarbeitet Array als Tabelle.

```csharp
public bool ArrayAsTable { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // JSON-Layoutoptionen erstellen und ArrayAsTable auf true setzen
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Beispieldaten im JSON-Format (vereinfacht zur Demonstration)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // Importiere JSON-Daten in ein Arbeitsblatt
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


