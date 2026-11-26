---
title: "Worksheet.Zoom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Representa el factor de escala en porcentaje. Debe estar entre 10 y 400."
type: docs
url: /es/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

```csharp
public int Zoom { get; set; }
```

### Observaciones

Por favor, establezca primero el tipo de vista.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el factor de zoom al 120%
            worksheet.Zoom = 120;
            
            // Mostrar el factor de zoom actual
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


