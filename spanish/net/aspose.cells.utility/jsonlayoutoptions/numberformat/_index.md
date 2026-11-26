---
title: "JsonLayoutOptions.NumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Obtiene y establece el formato del valor numérico"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Obtiene y establece el formato del valor numérico.

```csharp
public string NumberFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crear cadena de datos JSON
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Crear JsonLayoutOptions con NumberFormat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // Crear libro de trabajo a partir de JSON
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // Guardar en Excel
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


