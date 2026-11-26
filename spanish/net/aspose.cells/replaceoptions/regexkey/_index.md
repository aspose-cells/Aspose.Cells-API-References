---
title: "ReplaceOptions.RegexKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReplaceOptions. Indica si la clave buscada es una expresión regular. Si es true, la clave buscada se tomará como expresión regular"
type: docs
url: /es/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indica si la clave buscada es una expresión regular. Si es true, la clave buscada se tomará como expresión regular.

```csharp
public bool RegexKey { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Crear opciones de reemplazo con expresión regular
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Reemplazar todas las palabras que comienzan con 'p' o 'b' seguidas de una vocal
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Realizar el reemplazo
            workbook.Replace(pattern, replacement, options);

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


