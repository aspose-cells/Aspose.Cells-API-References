---
title: "Shape.IsWordArt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si esta forma es un WordArt"
type: docs
url: /es/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Indica si esta forma es un word art.

```csharp
public bool IsWordArt { get; }
```

### Observaciones

Solo para la forma heredada de archivo xls.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma WordArt con todos los parámetros requeridos
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Agregar una forma rectangular regular con todos los parámetros requeridos
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Verificar si las formas son WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // Ejemplo de uso de la propiedad IsWordArt
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


