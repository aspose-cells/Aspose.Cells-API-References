---
title: "Shape.IsSmartArt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si la forma es un smart art"
type: docs
url: /es/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Indica si la forma es un smart art.

```csharp
public bool IsSmartArt { get; }
```

### Observaciones

Solo para archivo ooxml.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma SmartArt (Nota: Aspose.Cells no expone directamente la creación de SmartArt en las versiones actuales)
            // Para la demostración, verificaremos las formas existentes
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Verificar si la forma es SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


