---
title: "ScrollBar.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Indica si la forma tiene sombreado 3D"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Indica si la forma tiene sombreado 3-D.

```csharp
public bool Shadow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento horizontal
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Establecer propiedades de la barra de desplazamiento
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Demostrar la propiedad Shadow
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Crear otra barra de desplazamiento para comparar
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Guarda el libro de trabajo
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


