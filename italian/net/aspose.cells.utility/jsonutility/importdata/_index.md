---
title: "JsonUtility.ImportData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo JsonUtility. Importa la stringa json"
type: docs
url: /it/net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Importa la stringa json.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| json | String | La stringa json. |
| celle | Celle | Le Cells. |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |
| opzione | JsonLayoutOptions | Le opzioni di importazione della stringa json. |

### Esempi

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

### Vedi anche

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


