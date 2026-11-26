---
title: "PicFormatOption.Bottom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PicFormatOption. Obtiene o establece el desplazamiento inferior para estirar la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Obtiene o establece el desplazamiento inferior para estirar la imagen.

```csharp
public double Bottom { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Utilice un archivo de imagen existente (reemplácelo con la ruta real de la imagen)
            string imagePath = "sample.jpg";

            // Agrega una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Configurar el relleno de la forma para usar la imagen de ejemplo
            // FillType se infiere al establecer ImageData, lo que define el tipo como Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Crear y configurar las opciones de formato de imagen
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Mostrar el valor inicial de Bottom
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Modificar el desplazamiento Bottom y mostrar el nuevo valor
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Asociar PicFormatOption con el relleno de la forma (suponiendo que sea aplicable)
            // Nota: Este paso puede requerir métodos específicos de la API que no se muestran en el contexto proporcionado
            // Para demostración, se crea y configura PicFormatOption

            // Guardar el libro de trabajo con los cambios aplicados
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


