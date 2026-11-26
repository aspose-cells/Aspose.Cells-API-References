---
title: "MsoLineFormatHelper.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormatHelper. Возвращает объект Style, представляющий стиль указанного диапазона"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Возвращает объект Style, который представляет стиль указанного диапазона.

```csharp
public MsoLineStyle Style { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Получить формат линии напрямую (MsoLineFormatHelper, по-видимому, является вспомогательным классом)
                // Поскольку мы не можем напрямую создать экземпляр MsoLineFormatHelper, будем работать со свойством LineFormat
                MsoLineFormat lineFormat = shape.LineFormat;

                // Отобразить текущее значение Style
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Установить новый стиль (поскольку Style доступен для чтения/записи)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Сохранить результат
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


