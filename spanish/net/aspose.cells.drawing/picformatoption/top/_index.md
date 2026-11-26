---
title: "PicFormatOption.Top"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PicFormatOption. Obtiene o establece el desplazamiento superior para estirar la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Obtiene o establece el desplazamiento superior para estirar la imagen.

```csharp
public double Top { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Utilice una imagen existente o proporcione la ruta correcta de la imagen
            string imagePath = "existingImage.png";

            // Agregar una forma con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Aplicar relleno de imagen usando ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Crear y configurar PicFormatOption directamente
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // Suponiendo que PicFormatOption necesita estar asociado con el formato de relleno
            // Esta parte podría requerir una implementación específica de la API que no se muestra en las definiciones de tipo
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


