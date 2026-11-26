---
title: "TextOptions.Outline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Representa el formato de contorno del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Representa el formato de contorno del texto.

```csharp
public LineFormat Outline { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma con texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Acceder a opciones de texto
            TextOptions textOptions = shape.TextOptions;

            // Configurar propiedades de contorno
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Guarda el libro de trabajo
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


