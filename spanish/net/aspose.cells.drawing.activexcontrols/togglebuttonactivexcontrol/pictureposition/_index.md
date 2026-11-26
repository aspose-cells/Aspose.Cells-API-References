---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Obtiene y establece la ubicación de la imagen del control relativa a su título"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Obtiene y establece la ubicación de la imagen del control relativa a su leyenda.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un control ActiveX ToggleButton con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Establezca la propiedad PicturePosition
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Establezca otras propiedades para demostrar la funcionalidad
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Guarda el libro de trabajo
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


