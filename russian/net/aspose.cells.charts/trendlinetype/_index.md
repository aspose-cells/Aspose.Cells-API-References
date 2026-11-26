---
title: "Перечисление TrendlineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.TrendlineType. Представляет тип линии тренда"
type: docs
url: /ru/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Представляет тип линии тренда.

```csharp
public enum TrendlineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Exponential | `0` | Экспоненциальный |
| Linear | `1` | Линейный |
| Logarithmic | `2` | Логарифмический |
| MovingAverage | `3` | MovingAverage |
| Polynomial | `4` | Polynomial |
| Power | `5` | Power |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Установка источника данных для категориальных данных NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Добавление различных типов линий тренда к диаграмме
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Сохранение файла Excel
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Добавление линии тренда указанного типа к указанному ряду
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Установка пользовательского названия линии тренда
            trendline.Name = trendlineName;
            
            // Отображение уравнения на диаграмме
            trendline.DisplayEquation = true;
            
            // Отображение значения R-квадрат на диаграмме
            trendline.DisplayRSquared = true;
            
            // Установка цвета линии тренда
            trendline.Color = Color.Red;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


