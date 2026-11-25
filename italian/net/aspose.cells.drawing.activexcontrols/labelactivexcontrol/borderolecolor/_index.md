---
title: "LabelActiveXControl.BorderOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LabelActiveXControl. Ottiene e imposta il colore ole dello sfondo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Ottiene e imposta il colore ole dello sfondo.

```csharp
public int BorderOleColor { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo Label ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl = 
                (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà
            labelControl.Caption = "Sample Label";
            labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
            labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Salva la cartella di lavoro
            workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");

            // Visualizza il colore del bordo
            Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
        }
    }
}
```

### Vedi anche

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


