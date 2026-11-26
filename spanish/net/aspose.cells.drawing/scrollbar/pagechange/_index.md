---
title: "ScrollBar.PageChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBar. Obtiene o establece el cambio de página"
type: docs
url: /es/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Obtiene o establece el cambio de página

```csharp
public int PageChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Mostrar el valor de la propiedad PageChange para demostrar que se guardó/cargó correctamente
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Ver también

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


