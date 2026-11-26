---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Получает и задает специальный эффект элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

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
    public class ListBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ListBox ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Установить свойство SpecialEffect
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // Проверить и вывести значение свойства SpecialEffect
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Сохраните книгу
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


