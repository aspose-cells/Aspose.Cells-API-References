---
title: "CheckBoxActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. Kontrol içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/iswordwrapped/
---
## CheckBoxActiveXControl.IsWordWrapped property

Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını belirtir.

```csharp
public bool IsWordWrapped { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 150, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "This is a long caption that should word wrap when enabled";
            checkBox.IsWordWrapped = true;
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


