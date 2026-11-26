---
title: "Shape.GetActualBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Obtiene la posición y el tamaño reales de la forma después de aplicar rotación, volteo, etc."
type: docs
url: /es/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Obtén la posición y el tamaño reales de la forma (después de aplicar rotación, volteo, etc.)

```csharp
public float[] GetActualBox()
```

### Valor de retorno

Devuelve la posición y el tamaño en el orden de x, y, w, h

### Observaciones

Nota: La interfaz no está completamente funcional, especialmente la información de ubicación no es correcta. Se recomienda no usar esta interfaz hasta que la función esté completa.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Obtenga las dimensiones reales del cuadro de la forma
            float[] box = rectangle.GetActualBox();

            // Muestra las dimensiones del cuadro
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Guarda el libro de trabajo
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


