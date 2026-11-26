---
title: "ScrollBar.CurrentValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Obtiene o establece el valor actual"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

Obtiene o establece el valor actual.

```csharp
public int CurrentValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento a la hoja de cálculo
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Establecer propiedades de la barra de desplazamiento usando los nombres de propiedades correctos
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Establecer y demostrar la propiedad CurrentValue
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Cambiar el valor actual
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


