---
title: "Shape.TextOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa las opciones de texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Representa las opciones de texto de la forma.

```csharp
public TextOptions TextOptions { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Establecer texto para la forma
            shape.Text = "Sample Text";

            // Acceda y modifique TextOptions
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


