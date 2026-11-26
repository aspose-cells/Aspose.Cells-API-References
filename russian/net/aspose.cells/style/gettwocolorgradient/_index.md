---
title: "Style.GetTwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Получить настройку двухцветного градиента"
type: docs
url: /ru/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Получить настройку двухцветного градиента.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | Color& | Один цвет градиента. |
| color2 | Color& | Два цвета градиента. |
| gradientStyleType | GradientStyleType& | Стиль затенения градиента. |
| variant | Int32& | Вариант градиента. |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Style.GetTwoColorGradientSetting(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль и задайте двухцветный градиент
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Подготовьте переменные для получения параметров градиента
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Вызовите метод GetTwoColorGradient
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Отобразите полученные параметры градиента
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Сохраните книгу
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


