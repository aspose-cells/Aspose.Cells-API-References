---
title: "TextBoxActiveXControl.IntegralHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger om kontrollen endast visar hela textrader utan att visa några delvisa rader"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/
---
## TextBoxActiveXControl.IntegralHeight property

Indikerar om kontrollen endast visar hela textrader utan att visa några partiella rader.

```csharp
public bool IntegralHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll och hämta dess ActiveXControl-egenskap
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera IntegralHeight-egenskapen
            Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
            
            // Ställ in IntegralHeight till true om den är false
            if (!textBox.IntegralHeight)
            {
                textBox.IntegralHeight = true;
                Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
            }

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


