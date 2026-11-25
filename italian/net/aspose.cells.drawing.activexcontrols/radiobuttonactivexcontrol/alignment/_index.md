---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RadioButtonActiveXControl. Ottiene e imposta la posizione della Caption rispetto al controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Ottiene e imposta la posizione della didascalia rispetto al controllo.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una nuova raccolta di forme e aggiungi il controllo ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Imposta la proprietà Alignment
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Salva la cartella di lavoro
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


