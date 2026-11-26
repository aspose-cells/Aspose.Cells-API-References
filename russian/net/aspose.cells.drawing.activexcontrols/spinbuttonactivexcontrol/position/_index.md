---
title: "SpinButtonActiveXControl.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SpinButtonActiveXControl. Получает и задает значение"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Получает и задает значение.

```csharp
public int Position { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте SpinButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // Получите ActiveX control и задайте свойство Position
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Сохраните книгу
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### См. также

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


