---
title: "ActiveXControl.IMEMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Получает и задает режим работы по умолчанию редактора ввода (IME) для элемента управления при получении им фокуса"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Получает и задает режим выполнения по умолчанию редактора ввода (Input Method Editor) для элемента управления при получении фокуса.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ActiveX ToggleButton с правильными координатами
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Установить свойства, включая IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Проверить и вывести свойство IMEMode
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Сохраните книгу
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


