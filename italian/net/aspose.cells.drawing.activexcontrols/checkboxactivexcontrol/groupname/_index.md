---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene e imposta il nome del gruppo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Ottiene e imposta il nome del gruppo.

```csharp
public string GroupName { get; set; }
```

### Esempi

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
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CheckBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà GroupName
            checkBox.GroupName = "Sheet1";

            // Verifica e visualizza il GroupName
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


