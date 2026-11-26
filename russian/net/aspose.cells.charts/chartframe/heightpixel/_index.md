---
title: "ChartFrame.HeightPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает высоту кадра в пикселях"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Получает или задает высоту кадра в пикселях.

```csharp
public virtual int HeightPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Получить доступ к заголовку диаграммы (который является ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Отобразить текущую высоту в пикселях
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Установить новую высоту для заголовка
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Получить доступ к легенде (другой ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Отобразить и изменить высоту легенды
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Сохраните книгу
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


