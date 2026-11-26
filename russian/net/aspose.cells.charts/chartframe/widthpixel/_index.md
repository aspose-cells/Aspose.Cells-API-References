---
title: "ChartFrame.WidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает ширину рамки в единицах пикселей"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

Получает или задает ширину кадра в пикселях.

```csharp
public virtual int WidthPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Получите заголовок диаграммы (который наследуется от ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Отобразить текущее значение WidthPixel заголовка диаграммы
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Установить новую ширину заголовка диаграммы в пикселях
            chart.Title.WidthPixel = 300;
            
            // Отобразить новое значение WidthPixel
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Сохраните книгу
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


