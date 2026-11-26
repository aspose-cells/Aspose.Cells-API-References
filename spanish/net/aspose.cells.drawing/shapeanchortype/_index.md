---
title: "Enum ShapeAnchorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.ShapeAnchorType. Representa el tipo de anclaje"
type: docs
url: /es/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Representa el tipo de ancla.

```csharp
public enum ShapeAnchorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| TwoCellAnchor | `0` | Representa un marcador de posición de anclaje de dos celdas |
| OneCellAnchor | `1` | Representa un marcador de posición de anclaje de una celda |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de grupo
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Demostrar el uso de ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Guarda el libro de trabajo
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


