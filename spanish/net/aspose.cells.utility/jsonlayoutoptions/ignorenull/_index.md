---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Indica si se ignora el valor nulo"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Indica si se ignora el valor nulo.

```csharp
public bool IgnoreNull { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // JSON de ejemplo con valores nulos
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // Configurar opciones de importación JSON con IgnoreNull establecido en true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // Importa datos JSON a la hoja de cálculo
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // Verificar los datos importados (la dirección nula debe ser ignorada)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // Guarda el libro de trabajo
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


