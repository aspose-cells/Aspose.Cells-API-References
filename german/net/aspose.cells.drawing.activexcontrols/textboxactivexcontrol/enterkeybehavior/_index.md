---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt das Verhalten der ENTER-Taste an. True gibt an, dass das Drücken von ENTER eine neue Zeile erzeugt. False gibt an, dass das Drücken von ENTER den Fokus zum nächsten Objekt in der Tab‑Reihenfolge verschiebt."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

Gibt das Verhalten der EINGABETASTE an. Wahr bedeutet, dass das Drücken von EINGABE eine neue Zeile erzeugt. Falsch bedeutet, dass das Drücken von EINGABE den Fokus zum nächsten Objekt in der Tab-Reihenfolge verschiebt.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX-Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die EnterKeyBehavior-Eigenschaft
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // Umschalten Sie die EnterKeyBehavior
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


