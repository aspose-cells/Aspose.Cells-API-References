---
title: ActiveXControlBase.Workbook
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets the Workbook object
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Gets the `Workbook` object.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {

            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape s = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 20);
            ComboBoxActiveXControl c = (ComboBoxActiveXControl)s.ActiveXControl;
            s.ActiveXControl.IsLocked = false;
            c.IsVisible = true;
            c.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.None;
            c.Font.Name = "Arial";
            c.Font.Color = System.Drawing.Color.Black;
            c.ListRows = 12;
            c.MatchEntry = Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType.None;

            // Save modified workbook
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


