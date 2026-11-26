---
title: "SpinButtonActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "SpinButtonActiveXControl property. Получает тип элемента управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

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
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте элемент управления SpinButton ActiveX (параметры: left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Проверьте тип элемента управления, используя свойство Type
            if (spinButton.Type == ControlType.SpinButton)
            {
                // Задайте некоторые свойства, специфичные для SpinButton
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Сохраните книгу
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


