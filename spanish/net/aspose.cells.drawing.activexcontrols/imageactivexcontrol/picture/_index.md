---
title: "ImageActiveXControl.Picture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene y establece los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] Picture { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX Image
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Establecer propiedades
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Establecer la propiedad Picture (usando una matriz de bytes de una imagen de muestra)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Verificar que la propiedad Picture se haya establecido
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


