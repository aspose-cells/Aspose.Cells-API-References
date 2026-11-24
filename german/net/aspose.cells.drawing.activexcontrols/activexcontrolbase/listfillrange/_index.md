---
title: "ActiveXControlBase.ListFillRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt den Listenausfüllbereich"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

Ruft den Listenfüllbereich ab und legt ihn fest.

```csharp
public string ListFillRange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für ListFillRange hinzufügen
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // Ein ComboBoxActiveXControl hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze ListFillRange, um das Kombinationsfeld zu füllen
            comboBox.ListFillRange = "A2:A10";

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


