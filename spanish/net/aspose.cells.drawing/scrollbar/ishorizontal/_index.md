---
title: "ScrollBar.IsHorizontal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Indica si se trata de una barra de desplazamiento horizontal"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Indica si esta es una barra de desplazamiento horizontal.

```csharp
public bool IsHorizontal { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento horizontal
            Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
            ScrollBar scrollBar = (ScrollBar)scrollBarShape;
            scrollBar.IsHorizontal = true;

            // Agregar una barra de desplazamiento vertical para comparación
            Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
            ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
            verticalScrollBar.IsHorizontal = false;

            // Demostrar la propiedad IsHorizontal
            Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
            Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


