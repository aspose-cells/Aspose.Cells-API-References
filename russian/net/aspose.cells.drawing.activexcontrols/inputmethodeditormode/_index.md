---
title: "Перечисление InputMethodEditorMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode. Представляет режим выполнения по умолчанию редактора ввода (Input Method Editor)."
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Представляет режим выполнения по умолчанию для Input Method Editor.

```csharp
public enum InputMethodEditorMode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NoControl | `0` | Не управляет IME. |
| On | `1` | IME включён. |
| Off | `2` | IME выключен. Английский режим. |
| Disable | `3` | IME выключен. Пользователь не может включить IME с клавиатуры. |
| Hiragana | `4` | IME включён в режиме полноширинного хирагана. |
| Katakana | `5` | IME включён в режиме полноширинного катакана. |
| KatakanaHalf | `6` | IME включён в режиме полуширинного катакана. |
| AlphaFull | `7` | IME включён в режиме полноширинного буквенно-цифрового ввода. |
| Alpha | `8` | IME включён в режиме полуширинного буквенно-цифрового ввода. |
| HangulFull | `9` | IME включён в режиме полноширинного хангыль. |
| Hangul | `10` | IME включён в режиме полуширинного хангыль. |
| HanziFull | `11` | IME включён в режиме полноширинного хандзи. |
| Hanzi | `12` | IME включён в режиме полуширинного хандзи. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class InputMethodEditorModeDemo
    {
        public static void InputMethodEditorModeExample()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления TextBox ActiveX на лист
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Установить режим IME в полноширинный хирагана
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Установите другие свойства для демонстрации
            textBoxControl.Text = "This is a test.";
            textBoxControl.IsEnabled = true;
            textBoxControl.IsLocked = false;
            textBoxControl.IsTransparent = false;
            textBoxControl.IsAutoSize = true;
            textBoxControl.Width = 200;
            textBoxControl.Height = 50;
            textBoxControl.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            textBoxControl.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.White);
            textBoxControl.IsVisible = true;
            textBoxControl.Shadow = false;

            // Сохраните книгу
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


