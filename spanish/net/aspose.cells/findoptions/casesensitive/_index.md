---
title: "FindOptions.CaseSensitive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si la cadena buscada distingue mayúsculas y minúsculas"
type: docs
url: /es/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

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
    public class FindOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // Buscar "bc" con sensibilidad a mayúsculas
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


