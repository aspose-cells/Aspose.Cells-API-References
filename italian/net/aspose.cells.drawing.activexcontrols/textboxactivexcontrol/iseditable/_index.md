---
title: "TextBoxActiveXControl.IsEditable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se l'utente può digitare nel controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/
---
## TextBoxActiveXControl.IsEditable property

Indica se l'utente può digitare nel controllo.

```csharp
public bool IsEditable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà IsEditable
            Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
            
            // Attiva/disattiva la proprietà IsEditable
            textBox.IsEditable = !textBox.IsEditable;
            Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


