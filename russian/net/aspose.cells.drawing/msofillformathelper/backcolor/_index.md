---
title: "MsoFillFormatHelper.BackColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormatHelper. Получает и задает цвет заднего фона"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Получает и задает цвет фона файла.

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

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте метку, просто чтобы иметь некоторое содержимое на листе
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper не предоставляет публичный конструктор, используйте рефлексию для его создания
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Задайте BackColor известным цветом (например, LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Считайте значение BackColor и отобразите его
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // При желании вы также можете прочитать ForeColor, чтобы показать, что он остаётся по умолчанию
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Сохраните книгу – вспомогательный объект заливки не привязан к фигуре,
                // но сохранение демонстрирует, что код выполнился без ошибок.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


