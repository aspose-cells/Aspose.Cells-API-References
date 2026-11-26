---
title: "Перечисление DropButtonStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle. Представляет символ, отображаемый на кнопке раскрытия"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

Представляет символ, отображаемый на кнопке раскрытия.

```csharp
public enum DropButtonStyle
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Plain | `0` | Отображает кнопку без символа. |
| Arrow | `1` | Отображает кнопку со стрелкой вниз. |
| Ellipsis | `2` | Отображает кнопку с многоточием (...). |
| Reduce | `3` | Отображает кнопку с горизонтальной линией, похожей на символ подчёркивания. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Добавить несколько элементов в ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Сохраните книгу
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Вывести используемый DropButtonStyle
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


