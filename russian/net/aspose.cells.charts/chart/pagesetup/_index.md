---
title: "Chart.PageSetup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Представляет описание настройки страницы в этой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Представляет описание настройки страницы в этой диаграмме.

```csharp
public PageSetup PageSetup { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и вставьте некоторые данные для диаграммы
            Worksheet dataSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            dataSheet.Name = "DataSheet";
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);

            // Добавьте лист диаграммы
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Добавьте диаграмму на лист диаграммы
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Получите доступ к PageSetup диаграммы
            PageSetup pageSetup = chart.PageSetup;

            // Установить свойства настройки страницы
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Установите заголовок с текстом и изображением
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Установите нижний колонтитул
            pageSetup.SetFooter(0, "Page &P of &N");

            // Сохраните книгу
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


