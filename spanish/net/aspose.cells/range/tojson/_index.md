---
title: "Range.ToJson"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Convierte el rango a un valor JSON"
type: docs
url: /es/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Convertir el rango a valor JSON.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | JsonSaveOptions | Las opciones de conversión |

### Ejemplos

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
            
            // Datos de ejemplo
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

### Ver también

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


