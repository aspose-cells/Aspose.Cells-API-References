---
title: "ScrollBar.Max"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Obtiene o establece el valor máximo del rango de una barra de desplazamiento o spinner"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Obtiene o establece el valor máximo del rango de una barra de desplazamiento o spinner.

```csharp
public int Max { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una barra de desplazamiento a la hoja de cálculo
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Establecer propiedades de la barra de desplazamiento
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Mostrar información
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


