---
title: "Класс TwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.TwoColorGradient. Представляет градиент из двух цветов"
type: docs
url: /ru/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Представляет градиент из двух цветов.

```csharp
public class TwoColorGradient
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Получает и устанавливает первый цвет градиента. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Получает и устанавливает второй цвет градиента. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Получает и устанавливает стиль затенения градиента. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Получает и устанавливает вариант градиента. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Инициализировать TwoColorGradient с параметрами конструктора
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Изменить свойства градиента после инициализации
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Создать стиль ячейки и применить градиент
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Применить стиль к ячейке и добавить содержимое
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Отрегулировать размеры ячейки для видимости
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Сохранить результат с форматированием градиента
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


