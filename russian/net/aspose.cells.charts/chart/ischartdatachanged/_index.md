---
title: "Chart.IsChartDataChanged"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Определяет, изменился ли источник данных диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Определяет, изменился ли источник данных диаграммы.

```csharp
public bool IsChartDataChanged()
```

### Возвращаемое значение

Возвращает true, если диаграмма изменена, иначе возвращает false

### Примечания

Метод определяет изменения в источнике данных диаграммы перед рендерингом диаграммы в формат изображения. При первом вызове Chart.toImage данные источника диаграммы (например, XValuesParseData, ValuesParseData) будут записаны. Перед повторным вызовом метода Chart.toImage вызовите метод IsChartDataChanged, чтобы проверить, требуется ли повторный рендеринг диаграммы.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Проверьте, изменились ли данные диаграммы (должно быть false изначально)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Измените данные диаграммы
                worksheet.Cells["B2"].PutValue(15);

                // Снова проверьте, изменились ли данные диаграммы
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Вычислите диаграмму, чтобы обновить её
                chart.Calculate();

                // Проверьте после вычисления
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


