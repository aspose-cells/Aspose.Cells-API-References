---
title: "Klass JsonUtility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Utility.JsonUtility-klass. Representerar verktygsklassen för bearbetning av json"
type: docs
url: /sv/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Representerar verktygsklassen för bearbetning av JSON.

```csharp
public class JsonUtility
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [JsonUtility](jsonutility/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Exporterar området till json-fil. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Exporterar området till json-fil. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Importera json-strängen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Skapa en instans av JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Eftersom JsonUtility-klassen inte har några egenskaper eller metoder definierade i JSON,
            // vi kommer att demonstrera dess instansiering och potentiella användning i sammanhang.

            // Exempel: Antag att JsonUtility kan användas för att bearbeta JSON-data på något sätt.
            // Obs: Den faktiska användningen skulle bero på metoderna och egenskaperna som finns i den verkliga klassen.
            // Här demonstrerar vi bara instansieringen eftersom inga metoder eller egenskaper tillhandahålls.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Ytterligare kod för att demonstrera potentiell användning
            // Till exempel, om JsonUtility hade en metod för att bearbeta JSON, skulle den kunna se ut så här:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Eftersom inga metoder tillhandahålls, avslutar vi exemplet här.
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


