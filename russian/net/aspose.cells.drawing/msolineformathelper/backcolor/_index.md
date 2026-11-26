---
title: "MsoLineFormatHelper.BackColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormatHelper. Получает и задает цвет фона границы линии"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Получает и задает цвет задней линии границы.

```csharp
public Color BackColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // Отобразить текущее значение BackColor
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Установить новое значение BackColor (поскольку оно доступно для чтения/записи)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Сохранить результат
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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


