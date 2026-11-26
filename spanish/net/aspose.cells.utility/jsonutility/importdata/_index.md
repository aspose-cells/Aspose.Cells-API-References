---
title: "JsonUtility.ImportData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método JsonUtility. Importar la cadena json"
type: docs
url: /es/net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Importar la cadena json.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| json | String | La cadena json. |
| celdas | Celdas | Las Cells. |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |
| opción | JsonLayoutOptions | Las opciones de importación de la cadena json. |

### Ejemplos

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

### Ver también

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


