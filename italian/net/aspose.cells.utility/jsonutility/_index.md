---
title: "Classe JsonUtility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Utility.JsonUtility class. Rappresenta la classe di utilità per l'elaborazione del json"
type: docs
url: /it/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Rappresenta la classe di utilità per l'elaborazione di JSON.

```csharp
public class JsonUtility
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [JsonUtility](jsonutility/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Esportazione dell'intervallo in un file json. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Esportazione dell'intervallo in un file json. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Importa la stringa json. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Crea un'istanza di JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Poiché la classe JsonUtility non ha alcuna proprietà o metodo definito nel JSON,
            // dimostreremo la sua istanziazione e l'uso potenziale in modo contestuale.

            // Esempio: Supponendo che JsonUtility possa essere usato per elaborare dati JSON in qualche modo.
            // Nota: L'uso effettivo dipenderebbe dai metodi e dalle proprietà disponibili nella classe reale.
            // Qui, stiamo solo dimostrando l'istanziazione poiché non sono forniti metodi o proprietà.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Codice aggiuntivo per dimostrare l'uso potenziale
            // Ad esempio, se JsonUtility avesse un metodo per elaborare JSON, potrebbe apparire così:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Poiché non sono forniti metodi, concluderemo l'esempio qui.
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


