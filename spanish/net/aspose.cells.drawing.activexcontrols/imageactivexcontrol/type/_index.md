---
title: "ImageActiveXControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageActiveXControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/
---
## ImageActiveXControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un control Image ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Control Type: " + imageControl.Type);
            
            // Establecer algunas propiedades
            imageControl.IsAutoSize = false;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
            
            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


