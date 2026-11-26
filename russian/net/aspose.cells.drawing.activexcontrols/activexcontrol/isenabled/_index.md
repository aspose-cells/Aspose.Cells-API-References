---
title: "ActiveXControl.IsEnabled"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Указывает, может ли элемент управления получать фокус и реагировать на события, созданные пользователем"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/
---
## ActiveXControl.IsEnabled property

Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем.

```csharp
public bool IsEnabled { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsEnabledDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 1, 0, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
            checkBox.IsEnabled = true;
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;

            Console.WriteLine("IsEnabled state: " + checkBox.IsEnabled);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


