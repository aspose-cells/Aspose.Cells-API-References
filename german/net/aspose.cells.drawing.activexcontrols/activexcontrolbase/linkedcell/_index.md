---
title: "ActiveXControlBase.LinkedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt die verknüpfte Zelle"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Ruft die verknüpfte Zelle ab und legt sie fest.

```csharp
public string LinkedCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein SpinButtonActiveXControl zum ersten Arbeitsblatt hinzu
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Konfigurieren Sie die Eigenschaften des SpinButton
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Verknüpfen Sie das Steuerelement mit der Zelle A1
            spinButton.LinkedCell = "A1";

            // Setzen Sie den Wert der Zelle A1 so, dass er der Anfangsposition entspricht
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Speichere die Arbeitsmappe
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


