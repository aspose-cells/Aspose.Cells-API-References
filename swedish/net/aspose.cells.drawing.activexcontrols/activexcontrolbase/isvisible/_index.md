---
title: "ActiveXControlBase.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Anger om den här kontrollen är synlig"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

Anger om denna kontroll är synlig.

```csharp
public virtual bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // Spara arbetsboken
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


