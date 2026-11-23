---
title: "JsonUtility.ImportData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode JsonUtility. Importer la chaîne json"
type: docs
url: /fr/net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Importer la chaîne json.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| json | String | La chaîne json. |
| cellules | Cellules | Les cellules. |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |
| option | JsonLayoutOptions | Les options d'importation de la chaîne json. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodImportDataWithStringCellsInt32Int32JsonLayouDemo
    {
        public static void Run()
        {
            string jsonInput = "[{"
                              + "\"Name\" : \"Name\","
                              + "\"DisplayName\" : \"DisplayName\","
                              + "\"ShowDisplayName\" : false"
                              + "},"
                              + "{"
                              + "\"Name\" : \"Nameone\","
                              + "\"DisplayName\" : \"DisplayNameone\","
                              + "\"ShowDisplayName\" : true"
                              + "},"
                              + "{"
                              + "\"Name\" : \"Nametwo\","
                              + "\"DisplayName\" : \"DisplayNametwo\","
                              + "\"ShowDisplayName\" : false"
                              + "}]";

            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


