---
title: "Класс MsoLineFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.MsoLineFormat. Представляет форматирование линий и наконечников стрелок"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Представляет форматирование линии и наконечника стрелки.

```csharp
public class MsoLineFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Получает и задает цвет задней линии границы. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Получает или задает стиль штриха для указанной линии. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Получает и задает цвет передней линии границы. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Указывает, видим ли объект. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Возвращает объект Style, который представляет стиль указанного диапазона. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Возвращает или задает толщину линии в единицах pt. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Создайте новый Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму дуги в лист
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Получите объект MsoLineFormat из формы
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Установите свойства объекта MsoLineFormat
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Сохраните книгу
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


