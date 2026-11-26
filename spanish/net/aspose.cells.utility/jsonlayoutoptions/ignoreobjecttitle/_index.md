---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Indica si se ignora el título cuando el objeto es una propiedad de otro objeto"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Indica si se ignora el título cuando el objeto es una propiedad de otro objeto.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
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

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos JSON de ejemplo con títulos de objetos
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // Crear JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Mostrar el valor actual de IgnoreObjectTitle
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Establecer para ignorar los títulos de objetos
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importar JSON con IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Guardar con títulos ignorados
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Restablecer la hoja de cálculo
            worksheet.Cells.Clear();

            // Establecer para incluir los títulos de objetos
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importar JSON con IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Guardar con títulos incluidos
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


