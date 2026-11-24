---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLayoutOptions-Konstruktor. Konstruktor zum Laden von JSON-Layout-Optionen"
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Konstruktor zum Laden von JSON-Layout-Optionen.

```csharp
public JsonLayoutOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Beispieldaten für JSON erstellen
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // JsonLayoutOptions mit dem Konstruktor initialisieren
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Optionen festlegen
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Importiere JSON-Daten in ein Arbeitsblatt
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


