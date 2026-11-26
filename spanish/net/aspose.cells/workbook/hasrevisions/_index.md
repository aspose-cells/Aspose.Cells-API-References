---
title: "Workbook.HasRevisions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene si el libro de trabajo tiene cambios rastreados"
type: docs
url: /es/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Obtiene si el libro de trabajo tiene cambios rastreados

```csharp
public bool HasRevisions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Realizar un cambio que creará una revisión
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Verificar si el libro de trabajo tiene revisiones
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Aceptar todas las revisiones (si las hay)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Verificar nuevamente después de aceptar revisiones
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


