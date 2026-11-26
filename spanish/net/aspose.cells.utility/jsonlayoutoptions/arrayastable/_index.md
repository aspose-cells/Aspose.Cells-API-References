---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Procesa Array como tabla"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Procesa la matriz como tabla.

```csharp
public bool ArrayAsTable { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear opciones de diseño JSON y establecer ArrayAsTable en true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Datos JSON de ejemplo (simplificados para demostración)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // Importa datos JSON a la hoja de cálculo
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


