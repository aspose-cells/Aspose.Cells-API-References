---
title: "Shape.InputRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene o establece el rango de la hoja de cálculo utilizado para rellenar el cuadro combinado especificado"
type: docs
url: /es/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Obtiene o establece el rango de hoja de cálculo utilizado para rellenar el cuadro combinado especificado.

```csharp
public string InputRange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Agregar una forma (rectángulo)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Establecer el rango de entrada para la forma
            shape.InputRange = "$A$1:$A$5";

            // Verificar y modificar el rango de entrada si es necesario
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


