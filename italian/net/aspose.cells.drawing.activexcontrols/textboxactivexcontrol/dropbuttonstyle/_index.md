---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Specifica il simbolo visualizzato sul pulsante a discesa"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Specifica il simbolo visualizzato sul pulsante a discesa

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo TextBox ActiveX
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Esegui il cast a TextBoxActiveXControl per accedere alle proprietà specifiche di TextBox
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Imposta la proprietà DropButtonStyle
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


