---
title: "Перечисление ControlScrollOrientation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation. Представляет тип ориентации прокрутки"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Представляет тип ориентации прокрутки.

```csharp
public enum ControlScrollOrientation
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Auto | `3` | Элемент управления отображается горизонтально, когда его ширина больше высоты. В противном случае элемент управления отображается вертикально. |
| Vertical | `0` | Элемент управления отображается вертикально. |
| Horizontal | `1` | Элемент управления отображается горизонтально. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте ScrollBarActiveXControl на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Установите свойства ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Продемонстрируйте установку ориентации с использованием перечисления ControlScrollOrientation
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Сохраните книгу
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


