---
title: "ImageActiveXControl.BorderStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene y establece el tipo de borde usado por el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/
---
## ImageActiveXControl.BorderStyle property

Obtiene y establece el tipo de borde utilizado por el control.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5, 5, 100, 100, 200, 200);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Establecer el estilo de borde y demostrar su uso
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black border

            // Establecer imagen de muestra (asegúrese de que este archivo exista en su directorio de ejecución)
            if (File.Exists("sample.png"))
            {
                imageControl.Picture = File.ReadAllBytes("sample.png");
            }

            workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


