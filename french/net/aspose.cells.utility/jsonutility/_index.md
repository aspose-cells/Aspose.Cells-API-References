---
title: "Classe JsonUtility"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Utility.JsonUtility. Représente la classe utilitaire de traitement du json"
type: docs
url: /fr/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Représente la classe utilitaire de traitement JSON.

```csharp
public class JsonUtility
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [JsonUtility](jsonutility/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Exportation de la plage vers un fichier json. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Exportation de la plage vers un fichier json. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Importer la chaîne json. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Créer une instance de JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Étant donné que la classe JsonUtility n'a aucune propriété ni méthode définie dans le JSON,
            // nous allons démontrer son instanciation et son utilisation potentielle de manière contextuelle.

            // Exemple : En supposant que JsonUtility pourrait être utilisé pour traiter des données JSON d'une certaine manière.
            // Remarque : L'utilisation réelle dépendrait des méthodes et propriétés disponibles dans la classe réelle.
            // Ici, nous ne faisons que démontrer l'instanciation car aucune méthode ni propriété n'est fournie.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Code supplémentaire pour démontrer une utilisation potentielle
            // Par exemple, si JsonUtility avait une méthode pour traiter le JSON, cela pourrait ressembler à ceci :
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Étant donné qu'aucune méthode n'est fournie, nous terminerons l'exemple ici.
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


