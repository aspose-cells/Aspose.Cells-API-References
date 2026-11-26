---
title: "Axis.CustomUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает пользовательское значение для единицы отображения"
type: docs
url: /ru/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Указывает пользовательское значение для единицы отображения.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство Axis.CustomDisplayUnit. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Доступ к оси значений
                Axis valueAxis = chart.ValueAxis;

                // Установить пользовательскую единицу отображения
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // Установить значение пользовательской единицы отображения
                valueAxis.CustomDisplayUnit = 1000000;

                // Отобразить значение свойства CustomUnit (устаревшее свойство)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // Сохраните книгу
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
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

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


