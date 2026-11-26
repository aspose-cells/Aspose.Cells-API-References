---
title: "CheckBoxActiveXControl.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Указывает, отмечен элемент управления или нет"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Указывает, отмечен элемент управления или нет.

```csharp
public CheckValueType Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления CheckBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Установите базовые свойства, включая Value
            checkBox.Caption = "Check Me";
            checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage

            // Сохраните книгу
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


