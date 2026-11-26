---
title: "PageSetup.Zoom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el factor de escala en porcentaje. Debe estar entre 10 y 400"
type: docs
url: /es/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

```csharp
public int Zoom { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el nivel de zoom al 150%
            worksheet.PageSetup.Zoom = 150;
            
            // Imprimir el nivel de zoom actual
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


