---
title: "JsonLayoutOptions.IgnoreArrayTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Indica si se ignora el título cuando el arreglo es una propiedad del objeto"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/
---
## JsonLayoutOptions.IgnoreArrayTitle property

Indica si se ignora el título cuando el arreglo es una propiedad del objeto.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad JsonLayoutOptions.IgnoreTitle. Esta propiedad será eliminada dentro de 6 meses a partir de febrero de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos JSON de muestra con títulos de arreglos
            string json = @"{
                ""Employees"": [
                    { ""Name"": ""John"", ""Age"": 30 },
                    { ""Name"": ""Jane"", ""Age"": 25 }
                ]
            }";

            // Crear JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Mostrar el valor actual de IgnoreArrayTitle
            Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);

            // Primera importación con IgnoreArrayTitle = false (predeterminado)
            options.IgnoreArrayTitle = false;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");

            // Borrar la hoja de cálculo para la segunda importación
            worksheet.Cells.Clear();

            // Segunda importación con IgnoreArrayTitle = true
            options.IgnoreArrayTitle = true;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");

            // Guarda el libro de trabajo
            workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


