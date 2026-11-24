---
title: "ActiveXControlBase.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Gibt an, ob dieses Steuerelement sichtbar ist"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

Gibt an, ob dieses Steuerelement sichtbar ist.

```csharp
public virtual bool IsVisible { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ListBox‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


