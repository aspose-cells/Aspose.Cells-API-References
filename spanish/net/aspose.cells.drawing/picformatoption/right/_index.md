---
title: "PicFormatOption.Right"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PicFormatOption. Obtiene o establece el desplazamiento derecho para estirar la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Obtiene o establece el desplazamiento derecho para estirar la imagen.

```csharp
public double Right { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con dimensiones especificadas
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Configurar el relleno de imagen para la forma
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // Acceder a las opciones de formato de imagen a través de TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Mostrar y modificar la propiedad Right
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Verificar el nuevo valor y guardar los cambios
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


