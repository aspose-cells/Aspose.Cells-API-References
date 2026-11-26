---
title: "Shape.WidthInShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Representa el ancho de la forma en unidades de 1/4000 de la forma padre"
type: docs
url: /es/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Representa el ancho de la forma, en unidades de 1/4000 de la forma padre.

```csharp
public int WidthInShape { get; set; }
```

### Observaciones

Solo se aplica cuando esta forma está en el grupo o gráfico.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear dos formas rectangulares
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Agrupa las formas usando objetos de forma
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Demuestra el uso de WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


