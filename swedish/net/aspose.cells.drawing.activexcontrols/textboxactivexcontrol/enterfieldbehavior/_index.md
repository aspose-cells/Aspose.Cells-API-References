---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger markeringsbeteende när kontrollen aktiveras. True anger att markeringen förblir oförändrad från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen aktiveras."
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Anger markeringsbeteendet när kontrollen aktiveras. True anger att markeringen förblir oförändrad från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen aktiveras.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX Control med korrekta parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera EnterFieldBehavior-egenskapen
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Växla EnterFieldBehavior-egenskapen
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Ställ in EnterFieldBehavior till true explicit
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


