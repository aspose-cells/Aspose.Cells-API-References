---
title: "LabelActiveXControl.Caption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LabelActiveXControl-Eigenschaft. Liest und schreibt den beschreibenden Text, der auf dem Steuerelement angezeigt wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/
---
## LabelActiveXControl.Caption property

Liest und setzt den beschreibenden Text, der auf einem Steuerelement angezeigt wird.

```csharp
public string Caption { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Label-ActiveX-Steuerelement hinzu
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Setze und demonstriere die Caption-Eigenschaft
            label.Caption = "Label1aaaa";
            
            // Speichern und neu laden, um die Persistenz zu überprüfen
            string path = "LabelActiveXDemo.xlsm";
            workbook.Save(path, SaveFormat.Xlsm);

            Workbook reopened = new Workbook(path);
            LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
            Console.WriteLine("Caption: " + reloadedLabel.Caption);
        }
    }
}
```

### Siehe auch

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


