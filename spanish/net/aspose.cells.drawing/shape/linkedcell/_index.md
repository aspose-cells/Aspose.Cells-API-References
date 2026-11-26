---
title: "Shape.LinkedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene o establece el rango de la hoja de cálculo vinculado al valor del control"
type: docs
url: /es/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Obtiene o establece el rango de la hoja de cálculo vinculado al valor del control.

```csharp
public string LinkedCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Establecer la propiedad LinkedCell a B6
            shape.LinkedCell = "$B$6";

            // Cambiar LinkedCell a A1 si era B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Mostrar el valor actual de LinkedCell
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


