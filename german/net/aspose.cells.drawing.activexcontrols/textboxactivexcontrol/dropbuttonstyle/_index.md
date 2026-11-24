---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyDropButtonStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein TextBox ActiveX-Steuerelement hinzu
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Wandeln Sie zu TextBoxActiveXControl um, um auf TextBox-spezifische Eigenschaften zuzugreifen
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Setzen Sie die DropButtonStyle-Eigenschaft
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


