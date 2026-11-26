---
title: "Перечисление ControlMatchEntryType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType. Представляет, как ListBox или ComboBox ищут в списке при вводе пользователем"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Представляет способ, которым ListBox или ComboBox ищет элементы списка при вводе пользователем.

```csharp
public enum ControlMatchEntryType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FirstLetter | `0` | Элемент управления ищет следующую запись, начинающуюся с введённого символа. При многократном вводе той же буквы происходит переключение между всеми записями, начинающимися с этой буквы. |
| Complete | `1` | По мере ввода каждого символа элемент управления ищет запись, соответствующую всем введённым символам. |
| None | `2` | Список не будет просматриваться, когда вводятся символы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Добавьте элемент управления ComboBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Добавить элементы в ComboBox
            comboBox.Value = "Apple;Banana;Cherry";

            // Добавить ActiveX‑элемент ListBox на лист
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Установить свойства для ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Добавить элементы в ListBox
            listBox.Value = "Apple;Banana;Cherry";

            // Сохраните книгу
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Выведите результаты
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


