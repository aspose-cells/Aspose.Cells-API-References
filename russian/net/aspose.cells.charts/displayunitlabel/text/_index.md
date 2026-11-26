---
title: "DisplayUnitLabel.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DisplayUnitLabel. Возвращает или задает текст метки единицы отображения"
type: docs
url: /ru/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Получает или задает текст метки единицы отображения.

```csharp
public override string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A1:A4", true);
            
            // Настроить метку единицы отображения
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Получить доступ и изменить текст метки единицы отображения
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Изменить текст
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Сохраните книгу
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### См. также

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


