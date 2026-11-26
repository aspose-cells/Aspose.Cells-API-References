---
title: "JsonLoadOptions.LayoutOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLoadOptions. Las opciones de importación de json"
type: docs
url: /es/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

Las opciones de importación de JSON.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyLayoutOptionsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga JSON con LayoutOptions
            JsonLoadOptions options = new JsonLoadOptions
            {
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // Crear un nuevo libro de trabajo con datos JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Datos JSON de ejemplo
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Importar JSON a la hoja de cálculo
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // Guarda el libro de trabajo
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


