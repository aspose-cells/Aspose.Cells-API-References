---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Получает и задает специальный эффект элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Получает и задает специальный эффект элемента управления.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ToggleButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Задать свойство SpecialEffect
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Сохраните книгу
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


