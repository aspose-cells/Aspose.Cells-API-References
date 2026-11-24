---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Ruft den Spezialeffekt des Steuerelements ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

Liest und setzt den Spezialeffekt des Steuerelements.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ListBox‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // SpecialEffect-Eigenschaft festlegen
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // Überprüfen und den SpecialEffect-Wert ausgeben
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


