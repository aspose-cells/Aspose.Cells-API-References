---
title: "TextBoxActiveXControl.IntegralHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement nur vollständige Textzeilen anzeigt, ohne teilweise Zeilen darzustellen."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/
---
## TextBoxActiveXControl.IntegralHeight property

Gibt an, ob das Steuerelement nur vollständige Textzeilen anzeigt, ohne Teilzeilen zu zeigen.

```csharp
public bool IntegralHeight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ActiveX-TextBox-Steuerelement hinzu und rufen Sie dessen ActiveXControl-Eigenschaft ab
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die IntegralHeight-Eigenschaft
            Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
            
            // Setzen Sie IntegralHeight auf true, wenn es false ist
            if (!textBox.IntegralHeight)
            {
                textBox.IntegralHeight = true;
                Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


