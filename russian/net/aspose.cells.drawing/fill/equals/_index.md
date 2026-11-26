---
title: "Fill.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Fill. /"
type: docs
url: /ru/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

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

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить прямоугольную фигуру на лист
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Получить объект FillFormat из фигуры
                FillFormat fillFormat1 = rectangle.Fill;

                // Создать другую фигуру, чтобы получить второй объект FillFormat
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Вызвать метод Equals для сравнения двух объектов FillFormat
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Отобразить результат сравнения
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Также продемонстрировать сравнение с null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Сохраните книгу
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


