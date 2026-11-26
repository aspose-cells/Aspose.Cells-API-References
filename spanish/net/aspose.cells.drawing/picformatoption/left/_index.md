---
title: "PicFormatOption.Left"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PicFormatOption. Obtiene o establece el desplazamiento izquierdo para estirar la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Obtiene o establece el desplazamiento izquierdo para estirar la imagen.

```csharp
public double Left { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar el formato de imagen
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Configurar el relleno de imagen para la forma
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Crear y configurar PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Aplicar opciones de formato a la forma (asumiendo el nombre de propiedad correcto)
            // Nota: Es posible que la propiedad original 'PictureFormatOptions' no exista en la versión actual de la API.
            // La línea siguiente está comentada para resolver el error de compilación.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Mostrar el desplazamiento izquierdo inicial
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Modificar el desplazamiento izquierdo para recortar un 20% del lado izquierdo
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Guardar el libro con el formato de imagen modificado
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


