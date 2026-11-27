---
title: "ComboBoxActiveXControl.SelectionMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Anger om användaren kan markera en textrad genom att klicka i området till vänster om texten"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/
---
## ComboBoxActiveXControl.SelectionMargin property

Anger om användaren kan markera en textrad genom att klicka i området till vänster om texten.

```csharp
public bool SelectionMargin { get; set; }
```

### Exempel

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

            // Demonstrera SelectionMargin-egenskapen
            comboBox.SelectionMargin = false;
            Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);

            // Växla och demonstrera igen
            comboBox.SelectionMargin = true;
            Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);

            workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


