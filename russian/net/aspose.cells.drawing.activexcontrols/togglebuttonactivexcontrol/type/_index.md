---
title: "ToggleButtonActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Получает тип ActiveX‑элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type/
---
## ToggleButtonActiveXControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ToggleButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Продемонстрировать использование свойства Type
            ControlType type = toggleButton.Type;
            Console.WriteLine("Control Type: " + type.ToString());

            // Установите некоторые свойства
            toggleButton.Caption = "Click Me";
            toggleButton.Value = CheckValueType.Checked;
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


