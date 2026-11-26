---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor JsonLayoutOptions. Constructor para cargar opciones de diseño JSON"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Constructor para cargar opciones de diseño JSON.

```csharp
public JsonLayoutOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear datos JSON de muestra
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Inicializar JsonLayoutOptions usando el constructor
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Establecer opciones
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Importa datos JSON a la hoja de cálculo
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


