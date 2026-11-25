---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Specifica il simbolo visualizzato sul pulsante a discesa"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Specifica il simbolo visualizzato sul pulsante a discesa

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà ShowDropButtonTypeWhen
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


