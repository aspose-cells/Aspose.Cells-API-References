---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger beteendet för ENTER-tangenten. True betyder att tryck på ENTER skapar en ny rad. False betyder att tryck på ENTER flyttar fokus till nästa objekt i tabb-ordningen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

Anger beteendet för ENTER-tangenten. True anger att tryck på ENTER skapar en ny rad. False anger att tryck på ENTER flyttar fokus till nästa objekt i tabb-ordningen.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX Control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera EnterKeyBehavior-egenskapen
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // Växla EnterKeyBehavior
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


