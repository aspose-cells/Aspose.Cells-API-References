---
title: "LabelActiveXControl.Caption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LabelActiveXControl proprietà. Ottiene e imposta il testo descrittivo che appare su un controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/
---
## LabelActiveXControl.Caption property

Ottiene e imposta il testo descrittivo che appare su un controllo.

```csharp
public string Caption { get; set; }
```

### Esempi

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

            // Aggiungi Label ActiveX Control
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Imposta e dimostra la proprietà Caption
            label.Caption = "Label1aaaa";
            
            // Salva e ricarica per verificare la persistenza
            string path = "LabelActiveXDemo.xlsm";
            workbook.Save(path, SaveFormat.Xlsm);

            Workbook reopened = new Workbook(path);
            LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
            Console.WriteLine("Caption: " + reloadedLabel.Caption);
        }
    }
}
```

### Vedi anche

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


