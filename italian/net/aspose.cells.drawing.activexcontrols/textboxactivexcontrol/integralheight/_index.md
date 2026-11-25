---
title: "TextBoxActiveXControl.IntegralHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/
---
## TextBoxActiveXControl.IntegralHeight property

Indica se il controllo mostrerà solo linee complete di testo senza visualizzare linee parziali.

```csharp
public bool IntegralHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox e ottieni la sua proprietà ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà IntegralHeight
            Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
            
            // Imposta IntegralHeight su true se è false
            if (!textBox.IntegralHeight)
            {
                textBox.IntegralHeight = true;
                Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


