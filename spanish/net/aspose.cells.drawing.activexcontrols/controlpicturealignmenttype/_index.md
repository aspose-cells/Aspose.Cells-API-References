---
title: "Enumeración ControlPictureAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType. Representa la alineación de la imagen dentro del Form o Image"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Representa la alineación de la imagen dentro del Formulario o Imagen.

```csharp
public enum ControlPictureAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| TopLeft | `0` | La esquina superior izquierda. |
| TopRight | `1` | La esquina superior derecha. |
| Center | `2` | El centro. |
| BottomLeft | `3` | La esquina inferior izquierda. |
| BottomRight | `4` | La esquina inferior derecha. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un ImageActiveXControl con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Establecer propiedades de la imagen
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Guarda el libro de trabajo
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


