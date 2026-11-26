---
title: "FindOptions.LookAtType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Tipo de búsqueda"
type: docs
url: /es/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Buscar tipo.

```csharp
public LookAtType LookAtType { get; set; }
```

### Observaciones

Cuando [`RegexKey`](../regexkey/) es true y el usuario ha especificado la regla exacta para la expresión regular, por consideraciones de rendimiento esta propiedad debe establecerse como EntireContent. De lo contrario, reformularemos la clave de búsqueda para garantizar que pueda coincidir según el tipo específico. Por ejemplo, cuando el tipo es Contains (este es el valor predeterminado para esta propiedad), añadiremos comodines al principio y al final de la clave de búsqueda automáticamente. En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y agrega algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Crear opciones de búsqueda con LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Buscar una fórmula que coincida exactamente con "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Cambiar a coincidencia parcial
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Ver también

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


