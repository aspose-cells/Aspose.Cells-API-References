---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl-egenskap. Hämtar och anger gruppens namn"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Hämtar och anger gruppens namn.

```csharp
public string GroupName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ange GroupName-egenskapen
            checkBox.GroupName = "Sheet1";

            // Verifiera och skriv ut GroupName
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Spara arbetsboken
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


