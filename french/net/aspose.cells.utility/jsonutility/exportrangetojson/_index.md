---
title: "JsonUtility.ExportRangeToJson"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode JsonUtility. Exportation de la plage vers un fichier json"
type: docs
url: /fr/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Exportation de la plage vers un fichier json.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage. |
| options | ExportRangeToJsonOptions | Les options d'exportation. |

### Valeur de retour

La valeur de la chaîne json.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode ExportRangeToJson(Range range, JsonSaveOptions options). Cette propriété sera supprimée 6 mois plus tard à partir de novembre 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer une plage couvrant les données
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Créez des options d'exportation
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // Exportez la plage vers JSON
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### Voir aussi

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Exportation de la plage vers un fichier json.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage. |
| options | JsonSaveOptions | Les options d'exportation. |

### Valeur de retour

La valeur de la chaîne json.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // Créer une plage (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // Configurer les options d'exportation JSON
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // Exportez la plage vers JSON
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // Afficher le résultat JSON
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### Voir aussi

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


