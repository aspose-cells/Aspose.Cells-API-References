---
title: "JsonUtility.ImportData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonUtility‑metod. Importera JSON‑strängen"
type: docs
url: /sv/net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Importera json-strängen.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| json | String | JSON‑strängen. |
| celler | Celler | Cellerna. |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |
| alternativ | JsonLayoutOptions | Alternativen för att importera JSON‑strängen. |

### Exempel

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

### Se även

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


