---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement vertikale Bildlaufleisten, horizontale Bildlaufleisten, beide oder keine hat"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Gibt an, ob das Steuerelement vertikale Bildlaufleisten, horizontale Bildlaufleisten, beides oder keine hat.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie eine neue Formsammlung und fügen Sie ein ActiveX-Steuerelement hinzu
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Die ScrollBars-Eigenschaft auf vertikal setzen
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


