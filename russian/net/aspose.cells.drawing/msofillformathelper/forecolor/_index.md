---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormatHelper. Получает и задает цвет переднего заливки"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Получает и задает основной цвет заливки.

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
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте метку, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Создайте экземпляр MsoFillFormatHelper с помощью рефлексии (нет публичного конструктора)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Отобразить значение ForeColor по умолчанию
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Задать новое значение ForeColor
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Продемонстрировать получение значения ForeColor
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Сохраните книгу, чтобы продемонстрировать успешное выполнение
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


