---
title: "TextBoxActiveXControl.IsEditable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger om användaren kan skriva i kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/
---
## TextBoxActiveXControl.IsEditable property

Indikerar om användaren kan skriva i kontrollen.

```csharp
public bool IsEditable { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera IsEditable-egenskapen
            Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
            
            // Växla IsEditable-egenskapen
            textBox.IsEditable = !textBox.IsEditable;
            Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);

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


