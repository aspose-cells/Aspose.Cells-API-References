---
title: "ActiveXControl.TextAlign"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Определяет, как выравнивать текст, используемый элементом управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

Представляет способ выравнивания текста, используемого элементом управления.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyTextAlignDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить два checkbox ActiveX контрола
            Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
            Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);

            // Получить ActiveX‑контролы
            CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
            CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;

            // Установить разные выравнивания текста
            checkbox1.TextAlign = TextAlignmentType.Center;
            checkbox2.TextAlign = TextAlignmentType.Right;

            // Отобразить значения выравнивания текста
            Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
            Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


