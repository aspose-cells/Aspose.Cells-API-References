---
title: "Перечисление FillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.FillType enum. Тип формата заливки"
type: docs
url: /ru/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Тип формата заливки.

```csharp
public enum FillType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Представляет тип автоматического форматирования. |
| None | `1` | Представляет тип отсутствующего форматирования. |
| Solid | `2` | Сплошной формат заливки. |
| Gradient | `3` | Градиентный формат заливки. |
| Texture | `4` | Текстурный формат заливки (включает заливку изображением). |
| Pattern | `5` | Шаблонный формат заливки. |
| Group | `6` | Наследовать свойства заливки группы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Установите тип заливки градиентом
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Добавить текстовое поле
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Установить тип градиентной заливки для текстового поля
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Сохраните книгу
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


