---
title: "Aufzählung ControlScrollBarType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType Aufzählung. Stellt den Typ der Bildlaufleiste dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Stellt den Typ der Bildlaufleiste dar.

```csharp
public enum ControlScrollBarType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Zeigt keine Bildlaufleisten an. |
| Horizontal | `1` | Zeigt eine horizontale Bildlaufleiste an. |
| BarsVertical | `2` | Zeigt eine vertikale Bildlaufleiste an. |
| BarsBoth | `3` | Zeigt sowohl eine horizontale als auch eine vertikale Bildlaufleiste an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ListBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die Eigenschaft ScrollBars, um sowohl horizontale als auch vertikale Bildlaufleisten anzuzeigen
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


