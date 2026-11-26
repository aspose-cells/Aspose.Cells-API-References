---
title: "ToggleButtonActiveXControl.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Указывает, отмечен элемент управления или нет"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

Указывает, отмечен элемент управления или нет.

```csharp
public CheckValueType Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ToggleButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Установите начальное значение в Unchecked
            toggleButton.Value = CheckValueType.UnChecked;

            // Проверьте и переключите значение, если оно Unchecked
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Сохраните книгу
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


