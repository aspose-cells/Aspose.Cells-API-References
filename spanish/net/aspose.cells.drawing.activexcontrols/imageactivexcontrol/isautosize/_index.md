---
title: "ImageActiveXControl.IsAutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Indica si el control redimensionará automáticamente para mostrar todo su contenido"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido.

```csharp
public override bool IsAutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un ImageActiveXControl a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5,  // left
                5,  // top
                100, // width
                100, // height
                0,   // imageWidth (0 for default)
                0    // imageHeight (0 for default)
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Establecer los datos de la imagen (asegúrese de que el archivo de imagen exista)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Demostrar la propiedad IsAutoSize
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


