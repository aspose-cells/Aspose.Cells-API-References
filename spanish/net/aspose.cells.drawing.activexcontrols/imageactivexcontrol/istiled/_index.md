---
title: "ImageActiveXControl.IsTiled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Indica si la imagen está en mosaico en el fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Indica si la imagen se repite en forma de mosaico en el fondo.

```csharp
public bool IsTiled { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsTiledDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control Image ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad IsTiled y otras propiedades
            imageControl.IsTiled = true;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;

            // Cargar una imagen desde un archivo (reemplazar con la ruta de su propia imagen)
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");

            Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
        }
    }
}
```

### Ver también

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


