---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions‑konstruktor. Konstruktor för att ladda JSON‑layoutalternativ"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Konstruktor för att ladda JSON‑layout‑alternativ.

```csharp
public JsonLayoutOptions()
```

### Exempel

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
            // Skapa exempel‑JSON‑data
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Initiera JsonLayoutOptions med hjälp av konstruktor
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Ställ in alternativ
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Importera JSON‑data till kalkylblad
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


