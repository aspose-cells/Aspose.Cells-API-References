---
title: "Перечисление ControlCaptionAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType. Представляет положение подписи относительно элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlcaptionalignmenttype/
---
## ControlCaptionAlignmentType enumeration

Представляет положение Caption относительно элемента управления.

```csharp
public enum ControlCaptionAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Left | `0` | Левая часть элемента управления. |
| Right | `1` | Правая часть элемента управления. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlCaptionAlignmentTypeDemo
    {
        public static void ControlCaptionAlignmentTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления CheckBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для CheckBox
            checkBox.Caption = "Check Me!";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Добавьте элемент управления RadioButton ActiveX на лист
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Установите свойства для RadioButton
            radioButton.Caption = "Select Me!";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Сохраните книгу
            workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
            workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
            // Выведите результаты
            Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
            Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


