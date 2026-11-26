---
title: "MsoLineFormatHelper.Weight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormatHelper. Возвращает или задает толщину линии в единицах pt"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Возвращает или задает толщину линии в единицах pt.

```csharp
public double Weight { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте форму для демонстрации форматирования линии
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Получить формат линии
                MsoLineFormat lineFormat = shape.LineFormat;

                // Отобразить текущее значение Weight
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Установить новое значение Weight (поскольку оно доступно для чтения/записи)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Сохранить результат
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


