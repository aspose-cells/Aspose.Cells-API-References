---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Ruft den Namen der Gruppe ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Liest und setzt den Namen der Gruppe.

```csharp
public string GroupName { get; set; }
```

### Beispiele

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
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein CheckBox‑ActiveX‑Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die GroupName-Eigenschaft
            checkBox.GroupName = "Sheet1";

            // Überprüfen und geben Sie den GroupName aus
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


