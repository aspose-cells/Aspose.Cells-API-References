---
title: "FindOptions.ValueTypeSensitive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada"
type: docs
url: /es/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar diferentes tipos de valor a las celdas
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // Crear opciones de búsqueda con ValueTypeSensitive = true
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // Buscar el número 100 (no encontrará la cadena "100")
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // Buscar la cadena "100" (no encontrará el número 100)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // Cambiar a ValueTypeSensitive = false
            options.ValueTypeSensitive = false;
            
            // Ahora ambas búsquedas encontrarán cualquier celda con "100" o 100
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


