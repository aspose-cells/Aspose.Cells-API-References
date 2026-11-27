---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger om fokus automatiskt flyttas till nästa kontroll när användaren har skrivit det maximala antalet tecken"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Indikerar om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken.

```csharp
public bool IsAutoTab { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX-kontroll och hämta dess kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera IsAutoTab-egenskapen
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // Ange IsAutoTab till true om den är false
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


