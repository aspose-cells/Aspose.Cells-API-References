---
title: "Shape.IsFilled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si el formato de relleno es visible"
type: docs
url: /es/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Indica si el formato de relleno es visible.

```csharp
public bool IsFilled { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Comprobar y modificar la propiedad IsFilled
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


