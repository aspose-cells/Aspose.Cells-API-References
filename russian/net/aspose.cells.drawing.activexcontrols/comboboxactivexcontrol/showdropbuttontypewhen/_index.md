---
title: "ComboBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает символ, отображаемый на кнопке раскрытия"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showdropbuttontypewhen/
---
## ComboBoxActiveXControl.ShowDropButtonTypeWhen property

Указывает символ, отображаемый на кнопке раскрытия

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            comboBox.ShowDropButtonTypeWhen = Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType.Always;
            comboBox.DropButtonStyle = Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle.Arrow;
            comboBox.Value = "Click the drop button";

            workbook.Save("ComboBoxShowDropButtonDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


