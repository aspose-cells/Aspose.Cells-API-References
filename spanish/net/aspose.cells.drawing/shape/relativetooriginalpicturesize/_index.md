---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si la forma es relativa al tamaño original de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Indica si la forma es relativa al tamaño original de la imagen.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Acceder a las propiedades de la forma - Picture ya es un Shape, no es necesario hacer cast
            Shape shape = picture;

            // Demostrar la propiedad RelativeToOriginalPictureSize
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Cambiar la propiedad
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


