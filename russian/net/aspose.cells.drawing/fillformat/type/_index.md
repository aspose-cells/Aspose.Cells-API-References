---
title: "FillFormat.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает и задает тип заливки"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Получает и задает тип заливки.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Отобразить текущее значение Type
            Console.WriteLine("Current Type value: " + fill.Type);

            // Изменить Type на Gradient (устаревшее свойство, используемое для демонстрации)
            fill.Type = FillType.Gradient;

            // Применить двухцветный градиентный эффект
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Сохранить изменённую книгу
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


