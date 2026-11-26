---
title: "ToggleButtonActiveXControl.Picture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Obtiene y establece los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] Picture { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un control ActiveX ToggleButton y obtenga su propiedad ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establezca la imagen para el botón de alternancia
            byte[] data = File.ReadAllBytes("image.png");
            toggleButton.Picture = data;

            // Guarda el libro de trabajo
            workbook.Save("ToggleButtonWithPicture.xlsx");
        }
    }
}
```

### Ver también

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


