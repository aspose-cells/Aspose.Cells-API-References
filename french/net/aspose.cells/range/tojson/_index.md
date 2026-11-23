---
title: "Range.ToJson"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Convertit la plage en valeur JSON"
type: docs
url: /fr/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Convertir la plage en valeur JSON.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | JsonSaveOptions | Les options de conversion |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToJsonWithJsonSaveOptionsDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            
            // Données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);

            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


