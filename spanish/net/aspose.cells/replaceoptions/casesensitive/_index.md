---
title: "ReplaceOptions.CaseSensitive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReplaceOptions. Indica si la cadena buscada distingue entre mayúsculas y minúsculas"
type: docs
url: /es/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indica si la cadena buscada distingue entre mayúsculas y minúsculas.

```csharp
public bool CaseSensitive { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Crear opciones de reemplazo con CaseSensitive = false
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Reemplazar todas las variaciones de mayúsculas y minúsculas de "apple" con "orange"
            workbook.Replace("apple", "orange", options);

            // Mostrar resultados
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Restablecer datos
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Cambiar a CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Mostrar resultados
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Ver también

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


