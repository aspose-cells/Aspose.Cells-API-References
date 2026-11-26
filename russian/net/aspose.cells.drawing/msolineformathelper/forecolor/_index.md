---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormatHelper. Получает и задает цвет линии границы"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Получает и задает цвет передней линии границы.

```csharp
public Color ForeColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // Отобразить текущее значение ForeColor
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Установить новое значение ForeColor (так как оно доступно для чтения/записи)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Сохранить результат
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


