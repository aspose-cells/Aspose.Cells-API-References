---
title: "JsonUtility.ImportData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonUtility-Methode. Importiert die JSON-Zeichenfolge"
type: docs
url: /de/net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Importiere die JSON-Zeichenkette.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| json | String | Der JSON-String. |
| Zellen | Zellen | Die Zellen. |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |
| Option | JsonLayoutOptions | Die Optionen zum Importieren des JSON-Strings. |

### Beispiele

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

### Siehe auch

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


