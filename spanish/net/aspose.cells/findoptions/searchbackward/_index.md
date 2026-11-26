---
title: "FindOptions.SearchBackward"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si se busca hacia atrás en las celdas"
type: docs
url: /es/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Indica si se busca hacia atrás en las celdas.

```csharp
public bool SearchBackward { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurar datos de muestra
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Buscar hacia adelante (comportamiento predeterminado)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Buscar hacia atrás
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


