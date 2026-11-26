---
title: "ScrollBar.IncrementalChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Obtiene o establece la cantidad en que la barra de desplazamiento o el spinner se incrementa una línea de desplazamiento"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Obtiene o establece la cantidad en que la barra de desplazamiento o el spinner se incrementa por desplazamiento de línea.

```csharp
public int IncrementalChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento a la hoja de cálculo
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Establecer propiedades de la barra de desplazamiento
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Mostrar las propiedades de la barra de desplazamiento
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Modificar el cambio incremental
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

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


