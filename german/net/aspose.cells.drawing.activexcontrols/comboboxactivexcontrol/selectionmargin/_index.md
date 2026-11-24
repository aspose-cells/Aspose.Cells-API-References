---
title: "ComboBoxActiveXControl.SelectionMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er in den Bereich links vom Text klickt"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/
---
## ComboBoxActiveXControl.SelectionMargin property

Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er links vom Text klickt.

```csharp
public bool SelectionMargin { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertySelectionMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // SelectionMargin-Eigenschaft demonstrieren
            comboBox.SelectionMargin = false;
            Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);

            // Umschalten und erneut demonstrieren
            comboBox.SelectionMargin = true;
            Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);

            workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


