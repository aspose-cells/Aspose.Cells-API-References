---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Hämtar och anger den speciella effekten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

Hämtar och anger den speciella effekten för kontrollen.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Ange SpecialEffect egenskap
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // Verifiera och skriv ut SpecialEffect‑värdet
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Spara arbetsboken
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


