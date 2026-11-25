---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Specifica il comportamento di selezione quando si entra nel controllo. True indica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False indica che tutto il testo nel controllo verrà selezionato quando si entra nel controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Specifica il comportamento di selezione quando si entra nel controllo. True indica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False indica che tutto il testo nel controllo verrà selezionato all'ingresso.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX con i parametri corretti
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà EnterFieldBehavior
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Attiva/disattiva la proprietà EnterFieldBehavior
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Imposta EnterFieldBehavior su true esplicitamente
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


