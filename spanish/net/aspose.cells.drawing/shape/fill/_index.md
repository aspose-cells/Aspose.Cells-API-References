---
title: "Shape.Fill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Devuelve un objeto FillFormat que contiene las propiedades de formato de relleno para la forma especificada"
type: docs
url: /es/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Devuelve un objeto [`FillFormat`](../fillformat/) que contiene las propiedades de formato de relleno para la forma especificada.

```csharp
public FillFormat Fill { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Obtener el formato de relleno de la forma
            FillFormat fillFmt = shape.Fill;

            // Establezca un relleno sólido con color
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Establecer transparencia
            fillFmt.Transparency = 0.5;

            // Guarda el libro de trabajo
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


