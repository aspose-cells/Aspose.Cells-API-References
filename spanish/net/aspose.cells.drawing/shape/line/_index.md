---
title: "Shape.Line"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el estilo de línea"
type: docs
url: /es/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Obtiene el estilo de línea

```csharp
public LineFormat Line { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea (devuelve LineShape directamente)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Acceder y modificar las propiedades de la línea
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Guarda el libro de trabajo
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


