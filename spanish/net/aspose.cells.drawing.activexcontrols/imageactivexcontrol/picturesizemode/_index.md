---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene y establece cómo mostrar la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Obtiene y establece cómo mostrar la imagen.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control Image ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Establecer PictureSizeMode y otras propiedades
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Cargar una imagen de muestra (reemplácela con la ruta de su propia imagen)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Mostrar el valor de PictureSizeMode
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Ver también

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


