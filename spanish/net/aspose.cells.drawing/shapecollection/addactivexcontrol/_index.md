---
title: "ShapeCollection.AddActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Crea un control Activex"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Crea un control Activex.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ControlType | El tipo del control. |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de Shape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de Shape, en unidades de píxel. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


