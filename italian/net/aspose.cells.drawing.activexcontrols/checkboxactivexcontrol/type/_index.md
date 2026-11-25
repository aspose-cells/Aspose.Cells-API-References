---
title: "CheckBoxActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CheckBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà
            checkBox.Caption = "Sample CheckBox";
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;
            checkBox.IsEnabled = true;

            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
            if (checkBox.Type == ControlType.CheckBox)
            {
                Console.WriteLine("This is a CheckBox control");
            }

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


