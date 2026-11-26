---
title: "LabelActiveXControl.PicturePosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece la ubicación de la imagen del control en relación con su título"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/
---
## LabelActiveXControl.PicturePosition property

Obtiene y establece la ubicación de la imagen del control relativa a su leyenda.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Demo Label";
            label.PicturePosition = ControlPicturePositionType.AboveLeft;
            
            Console.WriteLine("Label Picture Position: " + label.PicturePosition);
            
            workbook.Save("LabelActiveXControlPicturePositionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


