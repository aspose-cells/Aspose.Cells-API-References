---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Указывает, как указанный элемент управления будет отображать значения Null"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Указывает, как указанный элемент управления будет отображать значения Null.

```csharp
public bool IsTripleState { get; set; }
```

### Примечания

| **Настройка** | **Описание** |
| --- | --- |
| True | Элемент управления будет переключаться между состояниями для значений Да, Нет и Null. Элемент управления отображается затемнённым (с серым оттенком), когда его свойство Value установлено в Null. |
| False | (По умолчанию) Элемент управления будет переключаться между состояниями для значений Да и Нет. Значения Null отображаются так, как если бы они были значениями Нет. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ToggleButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Установите свойство IsTripleState в значение true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Измените свойство IsTripleState на false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Сохраните книгу
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### См. также

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


