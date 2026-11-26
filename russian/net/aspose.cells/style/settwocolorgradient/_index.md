---
title: "Style.SetTwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Устанавливает указанную заливку в двухцветный градиент"
type: docs
url: /ru/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Устанавливает указанную заливку в виде двухцветного градиента.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | Color | Один цвет градиента. |
| color2 | Color | Два цвета градиента. |
| gradientStyleType | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект стиля
            Style style = workbook.CreateStyle();

            // Установить двухцветный градиент для стиля
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Проверить настройки градиента
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Сохраните книгу
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


