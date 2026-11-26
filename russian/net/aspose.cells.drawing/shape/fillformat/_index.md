---
title: "Shape.FillFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает объект MsoFillFormat, который содержит свойства форматирования заливки для указанной фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Возвращает объект MsoFillFormat, который содержит свойства форматирования заливки для указанной фигуры.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Fill. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную фигуру, чтобы продемонстрировать свойство FillFormat
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Получите доступ к свойству FillFormat (только для чтения)
                MsoFillFormat fillFormat = shape.FillFormat;

                // Отобразите текущие свойства FillFormat
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // Измените свойства FillFormat (поскольку они не только для чтения)
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Отобразите обновлённые свойства FillFormat
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Сохраните книгу
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


