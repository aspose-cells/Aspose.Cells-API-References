---
title: "Enum ControlPicturePositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Représente l'emplacement de l'image du contrôle par rapport à sa légende"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Représente l'emplacement de l'image du contrôle par rapport à sa légende.

```csharp
public enum ControlPicturePositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LeftTop | `131072` | L'image apparaît à gauche de la légende. La légende est alignée avec le haut de l'image. |
| LeftCenter | `327683` | L'image apparaît à gauche de la légende. La légende est centrée par rapport à l'image. |
| LeftBottom | `524294` | L'image apparaît à gauche de la légende. La légende est alignée avec le bas de l'image. |
| RightTop | `2` | L'image apparaît à droite de la légende. La légende est alignée avec le haut de l'image. |
| RightCenter | `196613` | L'image apparaît à droite de la légende. La légende est centrée par rapport à l'image. |
| RightBottom | `393224` | L'image apparaît à droite de la légende. La légende est alignée avec le bas de l'image. |
| AboveLeft | `393216` | L'image apparaît au-dessus de la légende. La légende est alignée avec le bord gauche de l'image. |
| AboveCenter | `458753` | L'image apparaît au-dessus de la légende. La légende est centrée sous l'image. |
| AboveRight | `524290` | L'image apparaît au-dessus de la légende. La légende est alignée avec le bord droit de l'image. |
| BelowLeft | `6` | L'image apparaît en dessous de la légende. La légende est alignée avec le bord gauche de l'image. |
| BelowCenter | `65543` | L'image apparaît en dessous de la légende. La légende est centrée au-dessus de l'image. |
| BelowRight | `131080` | L'image apparaît en dessous de la légende. La légende est alignée avec le bord droit de l'image. |
| Center | `262148` | L'image apparaît au centre du contrôle. La légende est centrée horizontalement et verticalement au-dessus de l'image. |

### Exemples

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

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


