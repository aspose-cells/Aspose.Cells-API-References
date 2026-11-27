---
title: "Enum ControlPicturePositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Representerar placeringen av kontrollens bild i förhållande till dess rubrik"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Representerar placeringen av kontrollens bild relativt dess caption.

```csharp
public enum ControlPicturePositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LeftTop | `131072` | Bilden visas till vänster om rubriken. Rubriken är justerad med bildens överkant. |
| LeftCenter | `327683` | Bilden visas till vänster om rubriken. Rubriken är centrerad i förhållande till bilden. |
| LeftBottom | `524294` | Bilden visas till vänster om rubriken. Rubriken är justerad med bildens nederkant. |
| RightTop | `2` | Bilden visas till höger om rubriken. Rubriken är justerad med bildens överkant. |
| RightCenter | `196613` | Bilden visas till höger om rubriken. Rubriken är centrerad i förhållande till bilden. |
| RightBottom | `393224` | Bilden visas till höger om rubriken. Rubriken är justerad med bildens nederkant. |
| AboveLeft | `393216` | Bilden visas ovanför rubriken. Rubriken är justerad med bildens vänstra kant. |
| AboveCenter | `458753` | Bilden visas ovanför rubriken. Rubriken är centrerad under bilden. |
| AboveRight | `524290` | Bilden visas ovanför rubriken. Rubriken är justerad med bildens högra kant. |
| BelowLeft | `6` | Bilden visas under rubriken. Rubriken är justerad med bildens vänstra kant. |
| BelowCenter | `65543` | Bilden visas under rubriken. Rubriken är centrerad ovanför bilden. |
| BelowRight | `131080` | Bilden visas under rubriken. Rubriken är justerad med bildens högra kant. |
| Center | `262148` | Bilden visas i mitten av kontrollen. Rubriken är centrerad horisontellt och vertikalt ovanpå bilden. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


