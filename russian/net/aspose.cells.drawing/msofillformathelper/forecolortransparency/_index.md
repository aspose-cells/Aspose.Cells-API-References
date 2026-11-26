---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormatHelper. Возвращает или задает степень переднего цвета указанного заливки в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Возвращает или задает степень переднего цвета указанного заполнения как значение от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double ForeColorTransparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте метку, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Создайте экземпляр MsoFillFormatHelper с помощью рефлексии (нет публичного конструктора)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Отобразить значение ForeColorTransparency по умолчанию
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Задать новые значения ForeColor и ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Отобразить обновленные значения
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Продемонстрировать чтение значения прозрачности
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Сохраните книгу, чтобы продемонстрировать успешное выполнение
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


