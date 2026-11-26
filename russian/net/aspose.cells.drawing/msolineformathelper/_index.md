---
title: "Класс MsoLineFormatHelper"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.MsoLineFormatHelper. Представляет форматирование линий и наконечников стрелок"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Представляет форматирование линии и наконечника стрелки.

```csharp
public class MsoLineFormatHelper
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Получает и задает цвет задней линии границы. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Получает или задает стиль штриха для указанной линии. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Получает и задает цвет передней линии границы. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Указывает, видим ли объект. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Возвращает объект Style, который представляет стиль указанного диапазона. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Возвращает или задает толщину линии в единицах pt. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте форму для демонстрации форматирования линии
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Получите формат линии непосредственно из формы
                MsoLineFormat lineFormat = shape.LineFormat;

                // Установите свойства непосредственно в формате линии
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Отобразите настроенные свойства
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Сохраните книгу
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


