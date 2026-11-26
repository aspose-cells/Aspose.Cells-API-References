---
title: "Перечисление ShowDropButtonType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Указывает, когда отображать кнопку раскрытия"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Указывает, когда показывать кнопку раскрытия.

```csharp
public enum ShowDropButtonType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Never | `0` | Никогда не отображать кнопку раскрытия. |
| Focus | `1` | Отображать кнопку раскрытия, когда элемент управления в фокусе. |
| Always | `2` | Всегда отображать кнопку раскрытия. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установить свойства для элемента управления ComboBox ActiveX
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Добавить несколько элементов в ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Сохраните книгу
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


