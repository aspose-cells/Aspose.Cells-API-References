---
title: "ListBoxActiveXControl.BorderOleColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ListBoxActiveXControl propriété. Obtient et définit la couleur ole de l'arrière-plan"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderolecolor/
---
## ListBoxActiveXControl.BorderOleColor property

Obtient et définit la couleur ole de l'arrière-plan.

```csharp
public int BorderOleColor { get; set; }
```

### Exemples

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

### Voir aussi

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


