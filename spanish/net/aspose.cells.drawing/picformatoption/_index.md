---
title: "Clase PicFormatOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.PicFormatOption. Representa la opción de formato de imagen."
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Representa la opción de formato de imagen

```csharp
public class PicFormatOption
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PicFormatOption](picformatoption/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Obtiene o establece el desplazamiento inferior para estirar la imagen. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Obtiene o establece el desplazamiento izquierdo para estirar la imagen. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Obtiene o establece el desplazamiento derecho para estirar la imagen. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Obtiene o establece cuántas imágenes se apilan y escalan. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Obtiene o establece el desplazamiento superior para estirar la imagen. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Obtiene o establece el tipo de relleno de la imagen. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer el relleno de imagen
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // Propiedad FillType eliminada del acceso a MsoFillFormat
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Configurar opciones de formato de imagen
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Agregar segunda forma con imagen en mosaico
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // Propiedad FillType eliminada del acceso a MsoFillFormat
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


