---
title: "TextBoxActiveXControl.TabKeyBehavior"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se i caratteri di tabulazione sono consentiti nel testo del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/
---
## TextBoxActiveXControl.TabKeyBehavior property

Indica se i caratteri di tabulazione sono consentiti nel testo del controllo.

```csharp
public bool TabKeyBehavior { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX e ottieni la sua proprietà ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà TabKeyBehavior
            Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
            
            // Abilita TabKeyBehavior
            if (!textBoxControl.TabKeyBehavior)
            {
                textBoxControl.TabKeyBehavior = true;
                Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


