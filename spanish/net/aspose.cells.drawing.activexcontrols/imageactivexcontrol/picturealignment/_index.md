---
title: "ImageActiveXControl.PictureAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene y establece la alineación de la imagen dentro del Formulario o Imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/
---
## ImageActiveXControl.PictureAlignment property

Obtiene y establece la alineación de la imagen dentro del Formulario o Imagen.

```csharp
public ControlPictureAlignmentType PictureAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad PictureAlignment
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;

            // Cargar imagen de muestra (reemplácela con la ruta de la imagen real)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            workbook.Save("ImageActiveXControlDemo.xlsx");

            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
        }
    }
}
```

### Ver también

* enum [ControlPictureAlignmentType](../../controlpicturealignmenttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


