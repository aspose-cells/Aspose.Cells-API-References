---
title: "Clase ReplaceOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ReplaceOptions. Representa las opciones de reemplazo"
type: docs
url: /es/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Representa las opciones de reemplazo.

```csharp
public class ReplaceOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Indica si la cadena buscada distingue entre mayúsculas y minúsculas. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | La configuración de formato enriquecido para el texto reemplazado. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Indica si se debe coincidir con el contenido completo de las celdas |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Indica si la clave buscada es una expresión regular. Si es true, la clave buscada se tomará como expresión regular. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Obtiene y establece banderas de aplicación de configuraciones de fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Crear ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Reemplazar "Hello" con "Hi" en la hoja de cálculo
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Mostrar el número de reemplazos realizados
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Guarda el libro de trabajo
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


