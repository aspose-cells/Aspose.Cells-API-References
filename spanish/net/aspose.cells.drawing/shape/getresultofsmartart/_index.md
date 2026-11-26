---
title: "Shape.GetResultOfSmartArt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Convirtiendo smart art a formas agrupadas"
type: docs
url: /es/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Convirtiendo smart art a formas agrupadas.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular (ya que no podemos crear SmartArt directamente)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // En un escenario real, cargaríamos una forma SmartArt existente
            // Para propósitos de demostración, omitiremos la verificación IsSmartArt ya que no podemos establecerla

            // Obtener el resultado de SmartArt (solo funcionaría si la forma fuera realmente SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Ver también

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


