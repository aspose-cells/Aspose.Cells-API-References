---
title: "ImageActiveXControl.BorderOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene y establece el color ole del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/
---
## ImageActiveXControl.BorderOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public int BorderOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            imageControl.BorderOleColor = 0x0000FF; // Blue border
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;

            // Crear una imagen simple en memoria si el archivo de demostración no existe
            byte[] imageData;
            if (!File.Exists("demo.jpg"))
            {
                // Creación alternativa de imagen sin System.Drawing
                imageData = CreateSampleImage(100, 100);
            }
            else
            {
                imageData = File.ReadAllBytes("demo.jpg");
            }

            imageControl.Picture = imageData;
            workbook.Save("ImageActiveXControlBorderColorDemo.xlsx");

            Console.WriteLine($"Border color set to: {imageControl.BorderOleColor:X6}");
        }

        private static byte[] CreateSampleImage(int width, int height)
        {
            // Crear una imagen en escala de grises simple sin System.Drawing
            byte[] pixels = new byte[width * height * 3]; // RGB
            for (int i = 0; i < pixels.Length; i++)
            {
                pixels[i] = 200; // Light gray color
            }
            return pixels;
        }
    }
}
```

### Ver también

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


