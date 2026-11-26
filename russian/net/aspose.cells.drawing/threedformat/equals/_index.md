---
title: "ThreeDFormat.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreeDFormat."
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/equals/
---
## ThreeDFormat.Equals method

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру для сравнения 3D‑форматов
            Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);

            // Получить 3D‑форматы фигур
            ThreeDFormat format1 = shape1.ThreeDFormat;
            ThreeDFormat format2 = shape2.ThreeDFormat;

            // Настроить одинаковые 3D‑настройки
            format1.BottomBevelWidth = 10;
            format1.BottomBevelHeight = 10;
            format1.BottomBevelType = BevelType.ArtDeco;

            format2.BottomBevelWidth = 10;
            format2.BottomBevelHeight = 10;
            format2.BottomBevelType = BevelType.ArtDeco;

            try
            {
                // Вызовите метод Equals, чтобы сравнить 3D‑форматы
                bool areEqual = format1.Equals((object)format2);

                // Отобразить результат
                Console.WriteLine($"The 3D formats are equal: {areEqual}");

                // Измените одно свойство, чтобы они стали разными
                format2.BottomBevelWidth = 15;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("ThreeDFormatEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


