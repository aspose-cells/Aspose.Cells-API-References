---
title: "TextBoxActiveXControl.HideSelection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il fuoco"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/
---
## TextBoxActiveXControl.HideSelection property

Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il focus.

```csharp
public bool HideSelection { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà HideSelection
            Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
            
            // Imposta HideSelection su true se è false
            if (!textBox.HideSelection)
            {
                textBox.HideSelection = true;
                Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


