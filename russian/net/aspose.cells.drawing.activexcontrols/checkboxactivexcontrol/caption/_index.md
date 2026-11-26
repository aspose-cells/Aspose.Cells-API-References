---
title: "CheckBoxActiveXControl.Caption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Получает и задает описательный текст, отображаемый на элементе управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

Получает и задает описательный текст, отображаемый на элементе управления.

```csharp
public string Caption { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления CheckBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Установите и продемонстрируйте свойство Caption
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Сохраните книгу
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


