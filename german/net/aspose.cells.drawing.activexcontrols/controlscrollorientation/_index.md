---
title: "Enum ControlScrollOrientation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation enum. Gibt den Typ der Bildlauforientierung an."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Stellt den Typ der Bildlauforientierung dar

```csharp
public enum ControlScrollOrientation
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Auto | `3` | Das Steuerelement wird horizontal dargestellt, wenn seine Breite größer als seine Höhe ist. Andernfalls wird das Steuerelement vertikal dargestellt. |
| Vertical | `0` | Steuerelement wird vertikal dargestellt. |
| Horizontal | `1` | Steuerelement wird horizontal dargestellt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein ScrollBarActiveXControl zum ersten Arbeitsblatt hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Legen Sie Eigenschaften für das ScrollBarActiveXControl fest
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Demonstrieren Sie das Festlegen der Ausrichtung mit dem ControlScrollOrientation‑Enum
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


