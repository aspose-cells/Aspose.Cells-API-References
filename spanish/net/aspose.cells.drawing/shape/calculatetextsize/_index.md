---
title: "Shape.CalculateTextSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Recalcular el área de texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Recalcula el área de texto

```csharp
public int[] CalculateTextSize()
```

### Valor de retorno

Tamaño del texto en una matriz (ancho y alto).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un texto de ejemplo a la celda A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Crear una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Establecer texto en la forma
            shape.Text = "This is a test string to calculate text size";

            // Calcular el tamaño del texto
            int[] size = shape.CalculateTextSize();

            // Genere la salida de los resultados
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


