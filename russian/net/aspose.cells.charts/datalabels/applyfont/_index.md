---
title: "DataLabels.ApplyFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DataLabels. Применяет шрифт меток данных ко всем дочерним узлам"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Применить шрифт меток данных ко всем дочерним узлам.

```csharp
public void ApplyFont()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Создайте книгу и откройте первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Показать подписи данных
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Установите новый цвет шрифта для меток данных
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Примените настройки шрифта ко всем меткам данных
            series.DataLabels.ApplyFont();
            
            // Сохраните книгу
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


