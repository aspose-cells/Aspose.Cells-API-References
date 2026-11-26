---
title: "ScrollBar.Min"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Obtiene o establece el valor mínimo de una barra de desplazamiento o rango de spinner"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Obtiene o establece el valor mínimo del rango de una barra de desplazamiento o spinner.

```csharp
public int Min { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento a la hoja de cálculo
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Establecer propiedades de la barra de desplazamiento
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Mostrar el valor de la propiedad Min
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


