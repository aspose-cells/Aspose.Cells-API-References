---
title: "LabelActiveXControl.BorderOleColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LabelActiveXControl-Eigenschaft. Gibt die Ole-Farbe des Hintergrunds zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Liest und schreibt die OLE-Farbe des Hintergrunds.

```csharp
public int BorderOleColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Label-ActiveX-Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl = 
                (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            // Eigenschaften festlegen
            labelControl.Caption = "Sample Label";
            labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
            labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Speichere die Arbeitsmappe
            workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");

            // Die Rahmenfarbe anzeigen
            Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
        }
    }
}
```

### Siehe auch

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


