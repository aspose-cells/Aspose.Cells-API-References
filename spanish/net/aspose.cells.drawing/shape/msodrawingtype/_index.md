---
title: "Shape.MsoDrawingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el tipo de dibujo"
type: docs
url: /es/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Obtiene el tipo de dibujo.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma rectangular (parámetros corregidos)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Obtenga y muestre el MsoDrawingType de la forma
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Agregue una forma de línea (parámetros corregidos)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Obtenga y muestre el MsoDrawingType de la línea
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### Ver también

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


