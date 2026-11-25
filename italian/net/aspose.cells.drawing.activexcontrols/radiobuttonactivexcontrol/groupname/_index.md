---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RadioButtonActiveXControl. Ottiene e imposta il nome del gruppo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Ottiene e imposta il nome del gruppo.

```csharp
public string GroupName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi due controlli RadioButton ActiveX
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Imposta lo stesso nome del gruppo per renderli mutuamente esclusivi
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Imposta le didascalie
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Salva la cartella di lavoro
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


