---
title: "Worksheet.GridlineColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene y establece el color de la línea de cuadrícula"
type: docs
url: /es/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Obtiene y establece el color de la línea de cuadrícula

```csharp
public Color GridlineColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el color de la línea de cuadrícula a rojo
            worksheet.GridlineColor = Color.Red;
            
            // Guarda el libro de trabajo
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


