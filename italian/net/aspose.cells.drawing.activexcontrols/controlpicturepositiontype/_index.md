---
title: "Enum ControlPicturePositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Rappresenta la posizione dell'immagine del controllo rispetto alla sua didascalia"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Rappresenta la posizione dell'immagine del controllo rispetto alla sua didascalia.

```csharp
public enum ControlPicturePositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LeftTop | `131072` | L'immagine appare a sinistra della didascalia. La didascalia è allineata con la parte superiore dell'immagine. |
| LeftCenter | `327683` | L'immagine appare a sinistra della didascalia. La didascalia è centrata rispetto all'immagine. |
| LeftBottom | `524294` | L'immagine appare a sinistra della didascalia. La didascalia è allineata con la parte inferiore dell'immagine. |
| RightTop | `2` | L'immagine appare a destra della didascalia. La didascalia è allineata con la parte superiore dell'immagine. |
| RightCenter | `196613` | L'immagine appare a destra della didascalia. La didascalia è centrata rispetto all'immagine. |
| RightBottom | `393224` | L'immagine appare a destra della didascalia. La didascalia è allineata con la parte inferiore dell'immagine. |
| AboveLeft | `393216` | L'immagine appare sopra la didascalia. La didascalia è allineata con il bordo sinistro dell'immagine. |
| AboveCenter | `458753` | L'immagine appare sopra la didascalia. La didascalia è centrata sotto l'immagine. |
| AboveRight | `524290` | L'immagine appare sopra la didascalia. La didascalia è allineata con il bordo destro dell'immagine. |
| BelowLeft | `6` | L'immagine appare sotto la didascalia. La didascalia è allineata con il bordo sinistro dell'immagine. |
| BelowCenter | `65543` | L'immagine appare sotto la didascalia. La didascalia è centrata sopra l'immagine. |
| BelowRight | `131080` | L'immagine appare sotto la didascalia. La didascalia è allineata con il bordo destro dell'immagine. |
| Center | `262148` | L'immagine appare al centro del controllo. La didascalia è centrata orizzontalmente e verticalmente sopra l'immagine. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


