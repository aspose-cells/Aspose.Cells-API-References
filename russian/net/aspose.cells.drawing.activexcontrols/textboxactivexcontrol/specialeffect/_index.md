---
title: "TextBoxActiveXControl.SpecialEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Получает и задает специальный эффект элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/
---
## TextBoxActiveXControl.SpecialEffect property

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
    public class TextBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ActiveX‑элемент TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Задать свойство SpecialEffect
            textBox.SpecialEffect = ControlSpecialEffectType.Bump;

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


