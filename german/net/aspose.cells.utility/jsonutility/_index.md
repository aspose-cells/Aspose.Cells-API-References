---
title: "Klasse JsonUtility"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Utility JsonUtility Klasse. Stellt die Hilfsklasse zur Verarbeitung von JSON dar."
type: docs
url: /de/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Stellt die Hilfsklasse zur Verarbeitung von JSON dar.

```csharp
public class JsonUtility
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [JsonUtility](jsonutility/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Veraltet.**) Exportieren des Bereichs in eine JSON-Datei. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Exportieren des Bereichs in eine JSON-Datei. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Importiere die JSON-Zeichenkette. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Erstelle eine Instanz von JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Da die JsonUtility Klasse keine im JSON definierten Eigenschaften oder Methoden hat,
            // Wir werden seine Instanziierung und potenzielle Verwendung kontextbezogen demonstrieren.

            // Beispiel: Angenommen, JsonUtility könnte auf irgendeine Weise zur Verarbeitung von JSON-Daten verwendet werden.
            // Hinweis: Die tatsächliche Verwendung würde von den Methoden und Eigenschaften abhängen, die in der realen Klasse verfügbar sind.
            // Hier demonstrieren wir nur die Instanziierung, da keine Methoden oder Eigenschaften bereitgestellt werden.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Zusätzlicher Code, um die potenzielle Verwendung zu demonstrieren
            // Zum Beispiel, wenn JsonUtility eine Methode zur Verarbeitung von JSON hätte, könnte sie so aussehen:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Da keine Methoden bereitgestellt werden, beenden wir das Beispiel hier.
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


