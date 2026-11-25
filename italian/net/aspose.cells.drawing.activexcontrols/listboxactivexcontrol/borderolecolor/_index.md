---
title: "ListBoxActiveXControl.BorderOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Ottiene e imposta il colore ole dello sfondo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderolecolor/
---
## ListBoxActiveXControl.BorderOleColor property

Ottiene e imposta il colore ole dello sfondo.

```csharp
public int BorderOleColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 0, 0, 200, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            listBox.BorderOleColor = -2147483642;
            
            workbook.Save("ListBoxBorderOleColorDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


