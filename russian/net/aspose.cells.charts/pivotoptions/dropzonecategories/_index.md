---
title: "PivotOptions.DropZoneCategories"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotOptions. Указывает, отображается ли элемент управления для каждого поля PivotTable на оси строк PivotTable исходной таблицы на диаграмме, когда параметр dropZonesVisible установлен в значение true"
type: docs
url: /ru/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси строк исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Добавить диаграмму, использующую данные сводной таблицы
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Получить доступ к параметрам сводной таблицы из диаграммы
            PivotOptions options = chart.PivotOptions;
            
            // Продемонстрировать свойство DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Сохраните книгу
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


