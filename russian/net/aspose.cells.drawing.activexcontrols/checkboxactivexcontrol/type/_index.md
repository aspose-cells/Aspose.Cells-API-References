---
title: "CheckBoxActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Получает тип ActiveX‑элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

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
    public class CheckBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления CheckBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Установить свойства
            checkBox.Caption = "Sample CheckBox";
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;
            checkBox.IsEnabled = true;

            // Продемонстрировать использование свойства Type
            Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
            if (checkBox.Type == ControlType.CheckBox)
            {
                Console.WriteLine("This is a CheckBox control");
            }

            // Сохраните книгу
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


