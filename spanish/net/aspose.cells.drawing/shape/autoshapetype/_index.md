---
title: "Shape.AutoShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo de forma automática"
type: docs
url: /es/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Obtiene y establece el tipo de forma automática.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma a la hoja de cálculo con los parámetros correctos
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Verifique y modifique el AutoShapeType si es necesario
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Cambie el tipo de forma para demostrar la propiedad
            shape.AutoShapeType = AutoShapeType.Oval;

            // Guarda el libro de trabajo
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


