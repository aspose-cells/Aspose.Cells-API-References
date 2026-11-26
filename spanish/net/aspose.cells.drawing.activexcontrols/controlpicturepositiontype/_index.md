---
title: "Enum ControlPicturePositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Representa la ubicación de la imagen del control en relación con su título"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Representa la ubicación de la imagen del control relativa a su título.

```csharp
public enum ControlPicturePositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LeftTop | `131072` | La imagen aparece a la izquierda del título. El título está alineado con la parte superior de la imagen. |
| LeftCenter | `327683` | La imagen aparece a la izquierda del título. El título está centrado respecto a la imagen. |
| LeftBottom | `524294` | La imagen aparece a la izquierda del título. El título está alineado con la parte inferior de la imagen. |
| RightTop | `2` | La imagen aparece a la derecha del título. El título está alineado con la parte superior de la imagen. |
| RightCenter | `196613` | La imagen aparece a la derecha del título. El título está centrado respecto a la imagen. |
| RightBottom | `393224` | La imagen aparece a la derecha del título. El título está alineado con la parte inferior de la imagen. |
| AboveLeft | `393216` | La imagen aparece encima del título. El título está alineado con el borde izquierdo de la imagen. |
| AboveCenter | `458753` | La imagen aparece encima del título. El título está centrado debajo de la imagen. |
| AboveRight | `524290` | La imagen aparece encima del título. El título está alineado con el borde derecho de la imagen. |
| BelowLeft | `6` | La imagen aparece debajo del título. El título está alineado con el borde izquierdo de la imagen. |
| BelowCenter | `65543` | La imagen aparece debajo del título. El título está centrado encima de la imagen. |
| BelowRight | `131080` | La imagen aparece debajo del título. El título está alineado con el borde derecho de la imagen. |
| Center | `262148` | La imagen aparece en el centro del control. El título está centrado horizontal y verticalmente sobre la imagen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPicturePositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            activeXControl.Caption = "Demo Button";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.IsAutoSize = true;

            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


