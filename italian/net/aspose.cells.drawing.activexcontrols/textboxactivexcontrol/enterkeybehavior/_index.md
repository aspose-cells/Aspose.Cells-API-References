---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Specifica il comportamento del tasto ENTER. True indica che premendo ENTER verrà creata una nuova riga. False indica che premendo ENTER il focus si sposterà sull'oggetto successivo nell'ordine di tabulazione"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

Specifica il comportamento del tasto ENTER. True specifica che premere ENTER creerà una nuova riga. False specifica che premere ENTER sposterà il focus al prossimo oggetto nell'ordine di tabulazione.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterKeyBehaviorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà EnterKeyBehavior
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // Attiva/disattiva la EnterKeyBehavior
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

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


