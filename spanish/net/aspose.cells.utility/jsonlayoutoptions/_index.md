---
title: "Clase JsonLayoutOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Utility.JsonLayoutOptions. Representa las opciones del tipo de diseño json"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Representa las opciones del tipo de diseño JSON.

```csharp
public class JsonLayoutOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Constructor para cargar opciones de diseño JSON. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Procesa la matriz como tabla. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Indica si se convierte la cadena en json a un valor numérico o de fecha. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Obtiene y establece el formato del valor de fecha. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Indica si se ignora el título si la matriz es una propiedad del objeto. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Indica si se ignora el valor nulo. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Indica si se debe ignorar el título cuando el objeto es una propiedad de otro objeto. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ignora los títulos de los atributos |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Indica si se mantiene el esquema de este JSON. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Obtiene y establece el formato del valor numérico. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Obtiene y establece el estilo del título. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea JsonLayoutOptions y establece sus propiedades
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Datos JSON de ejemplo
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Importa datos JSON a la hoja de cálculo
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


