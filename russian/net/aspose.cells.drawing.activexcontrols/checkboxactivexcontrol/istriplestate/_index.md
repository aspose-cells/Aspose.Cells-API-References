---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Указывает, как указанный элемент управления будет отображать значения Null"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления CheckBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Настройте базовые свойства
            checkBox.Caption = "Triple State Demo";
            
            // Продемонстрировать свойство IsTripleState
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Сохраните книгу
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### См. также

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


