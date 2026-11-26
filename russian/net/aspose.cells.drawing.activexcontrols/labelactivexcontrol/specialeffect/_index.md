---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LabelActiveXControl property. Получает и задает специальный эффект элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

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
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления Label ActiveX с всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Установите базовые свойства
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // Продемонстрировать свойство SpecialEffect
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // Изменить SpecialEffect и показать разницу
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Сохраните книгу
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


