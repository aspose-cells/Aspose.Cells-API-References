---
title: "TextBoxActiveXControl.IsWordWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il contenuto del controllo si avvolge automaticamente alla fine di una riga"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/
---
## TextBoxActiveXControl.IsWordWrapped property

Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga.

```csharp
public bool IsWordWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta del testo che trarrebbe beneficio dall'interruzione di riga
            textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";

            // Verifica e imposta la proprietà IsWordWrapped
            if (!textBox.IsWordWrapped)
            {
                textBox.IsWordWrapped = true;
                Console.WriteLine("Word wrapping has been enabled for the TextBox.");
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


