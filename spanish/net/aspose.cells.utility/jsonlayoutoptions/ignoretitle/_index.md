---
title: "JsonLayoutOptions.IgnoreTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Ignora los títulos de los atributos"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/ignoretitle/
---
## JsonLayoutOptions.IgnoreTitle property

Ignora los títulos de los atributos

```csharp
public bool IgnoreTitle { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos JSON de ejemplo
            string jsonInput = @"{
                ""Products"": [
                    {
                        ""Name"": ""Product1"",
                        ""Price"": 100,
                        ""Date"": ""2023-01-15""
                    },
                    {
                        ""Name"": ""Product2"",
                        ""Price"": 200,
                        ""Date"": ""2023-02-20""
                    }
                ]
            }";

            // Establecer JsonLayoutOptions con IgnoreTitle = true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreTitle = true;  // This will skip the title row in output
            options.ArrayAsTable = true;
            options.DateFormat = "yyyy/MM/dd";

            // Importar datos JSON
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("output_ignore_title.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


