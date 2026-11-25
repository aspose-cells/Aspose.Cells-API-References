---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Ottiene e imposta un carattere da visualizzare al posto dei caratteri inseriti"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

Ottiene e imposta un carattere da visualizzare al posto dei caratteri inseriti.

```csharp
public char PasswordChar { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX e ottieni la sua forma
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // Ottieni il TextBoxActiveXControl dalla forma
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà PasswordChar
            textBoxControl.PasswordChar = '*';

            // Imposta del testo per dimostrare la mascheratura della password
            textBoxControl.Text = "password123";

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


