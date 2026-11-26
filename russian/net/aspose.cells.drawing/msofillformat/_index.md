---
title: "Класс MsoFillFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.MsoFillFormat. Представляет формат заливки для фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Представляет формат заполнения для фигуры.

```csharp
public class MsoFillFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Получает и задает цвет фона файла. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Получает и задает основной цвет заливки. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Получает и задает данные текстурного и графического заполнения. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Указывает, есть ли заполнение. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Получает тип текстурного заполнения. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |

## Методы

| Имя | Описание |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Устанавливает указанное заполнение в градиент из одного цвета. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму дуги в лист
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Получите доступ к формату заливки фигуры
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Установите основной цвет заливки
            fillFormat.ForeColor = Color.Blue;

            // Установите задний цвет заливки
            fillFormat.BackColor = Color.LightBlue;

            // Установите прозрачность
            fillFormat.Transparency = 0.5;

            // Проверьте, видима ли заливка
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Установите градиентную заливку одним цветом
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Сохраните книгу
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


