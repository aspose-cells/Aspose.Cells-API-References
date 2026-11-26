---
title: "Enum ControlPictureSizeMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Representa cómo mostrar la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Representa cómo mostrar la imagen.

```csharp
public enum ControlPictureSizeMode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Clip | `0` | Recorta cualquier parte de la imagen que sea más grande que los límites del control. |
| Stretch | `1` | Estira la imagen para llenar el área del control. Esta configuración distorsiona la imagen en la dirección horizontal o vertical. |
| Zoom | `3` | Amplía la imagen, pero no distorsiona la imagen en la dirección horizontal o vertical. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Agregar un ImageActiveXControl a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Establecer los datos de la imagen para el ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Establezca el PictureSizeMode a Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Establezca otras propiedades del ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Guarda el libro de trabajo
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


