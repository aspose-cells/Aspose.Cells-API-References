---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой рабочей книги их ссылке"
type: docs
url: /ru/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылкам.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установите PropertiesFollowChartPoint в значение true
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверьте, что настройка сохранена
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


