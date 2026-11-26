---
title: "Shape.TextVerticalOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo de desbordamiento vertical de texto de la forma que contiene texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

Obtiene y establece el tipo de desbordamiento vertical del texto de la forma que contiene texto.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // Establecer texto y hacer que desborde verticalmente
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


