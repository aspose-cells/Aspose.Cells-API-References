---
title: "Worksheet.HasAutofilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica si esta hoja de cálculo tiene filtro automático"
type: docs
url: /es/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Indica si esta hoja de cálculo tiene filtro automático.

```csharp
public bool HasAutofilter { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Establecer filtro automático
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Comprobar si la hoja de cálculo tiene filtro automático
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


