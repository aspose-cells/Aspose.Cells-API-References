---
title: "Перечисление ControlScrollBarType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType. Представляет тип полосы прокрутки"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Представляет тип полосы прокрутки.

```csharp
public enum ControlScrollBarType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Не отображает полосы прокрутки. |
| Horizontal | `1` | Отображает горизонтальную полосу прокрутки. |
| BarsVertical | `2` | Отображает вертикальную полосу прокрутки. |
| BarsBoth | `3` | Отображает как горизонтальную, так и вертикальную полосу прокрутки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ActiveX‑элемент ListBox на лист
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство ScrollBars, чтобы отображать как горизонтальные, так и вертикальные полосы прокрутки
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Сохраните книгу
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


