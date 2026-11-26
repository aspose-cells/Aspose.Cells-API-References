---
title: "Axis.CustUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает пользовательское значение для единицы отображения"
type: docs
url: /ru/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Указывает пользовательское значение для единицы отображения.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство Axis.CustomUnit. Это свойство будет удалено через 12 месяцев, начиная с января 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
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
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Добавьте диаграмму и задайте её диапазон данных
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Получить ось значений
            Axis valueAxis = chart.ValueAxis;

            // Отобразить текущее значение CustUnit (устаревшее свойство)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Установить новое значение пользовательской единицы (1 000 000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Отобразить новое значение CustUnit
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Сохранить результат
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


