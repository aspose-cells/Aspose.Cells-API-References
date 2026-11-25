---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Ottiene e imposta il tipo di bordo utilizzato dal controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

Ottiene e imposta il tipo di bordo utilizzato dal controllo.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà BorderStyle
            textBox.BorderStyle = ControlBorderType.Single;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


