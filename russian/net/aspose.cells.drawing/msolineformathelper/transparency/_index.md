---
title: "MsoLineFormatHelper.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormatHelper. Возвращает или задает степень прозрачности указанного заполнения значением от 0.0 (непрозрачно) до 1.0 (полностью прозрачно)"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
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

                // Отобразить текущее значение Transparency
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Установить новое значение Transparency (так как оно доступно для чтения/записи)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Сохранить результат
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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


