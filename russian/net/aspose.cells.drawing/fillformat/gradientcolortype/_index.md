---
title: "FillFormat.GradientColorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает тип градиентного цвета для указанной заливки"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Возвращает тип градиентного цвета для указанной заливки.

```csharp
public GradientColorType GradientColorType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму, чтобы продемонстрировать заливку градиентом
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Установить двухцветную градиентную заливку
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Получите доступ к FillFormat, чтобы получить GradientColorType
                FillFormat fillFormat = shape.Fill;

                // Отобразить значение GradientColorType
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Сохраните книгу
                workbook.Save("GradientColorTypeDemo.xlsx");
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

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


