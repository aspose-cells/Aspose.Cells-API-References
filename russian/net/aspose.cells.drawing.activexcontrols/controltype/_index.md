---
title: "Перечисление ControlType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Представляет все типы ActiveX‑контроля"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controltype/
---
## ControlType enumeration

Представляет все типы ActiveX‑контролей.

```csharp
public enum ControlType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| CommandButton | `0` | Кнопка |
| ComboBox | `1` | Выпадающий список |
| CheckBox | `2` | Флажок |
| ListBox | `3` | Список |
| TextBox | `4` | Текстовое поле |
| SpinButton | `5` | Спиннер |
| RadioButton | `6` | Радиокнопка |
| Label | `7` | Метка |
| Image | `8` | Изображение |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | Полоса прокрутки |
| BarCode | `11` | Полоса прокрутки |
| Unknown | `12` | Неизвестно |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlTypeDemo
    {
        public static void ControlTypeExample()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте CommandButton ActiveX control
            Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
            ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
            commandButtonControl.IsEnabled = true;
            commandButtonControl.IsVisible = true;

            // Добавить элемент управления ComboBox ActiveX
            Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
            ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
            comboBoxControl.IsEnabled = true;
            comboBoxControl.IsVisible = true;

            // Добавить элемент управления CheckBox ActiveX
            Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
            ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
            checkBoxControl.IsEnabled = true;
            checkBoxControl.IsVisible = true;

            // Добавьте ListBox ActiveX control
            Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
            ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
            listBoxControl.IsEnabled = true;
            listBoxControl.IsVisible = true;

            // Добавить элемент управления TextBox ActiveX
            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
            ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsVisible = true;

            // Добавьте SpinButton ActiveX control
            Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
            ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
            spinButtonControl.IsEnabled = true;
            spinButtonControl.IsVisible = true;

            // Добавьте RadioButton ActiveX control
            Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
            ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
            radioButtonControl.IsEnabled = true;
            radioButtonControl.IsVisible = true;

            // Добавьте Label ActiveX control
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
            ActiveXControl labelControl = labelShape.ActiveXControl;
            labelControl.IsEnabled = true;
            labelControl.IsVisible = true;

            // Добавьте Image ActiveX control
            Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
            ActiveXControl imageControl = imageShape.ActiveXControl;
            imageControl.IsEnabled = true;
            imageControl.IsVisible = true;

            // Добавьте ToggleButton ActiveX control
            Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
            ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
            toggleButtonControl.IsEnabled = true;
            toggleButtonControl.IsVisible = true;

            // Добавьте ScrollBar ActiveX control
            Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
            ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
            scrollBarControl.IsEnabled = true;
            scrollBarControl.IsVisible = true;
                       

            // Сохраните книгу
            workbook.Save("ControlTypeExample.xlsx");
            workbook.Save("ControlTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


