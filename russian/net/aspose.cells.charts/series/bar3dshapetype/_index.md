---
title: "Series.Bar3DShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает или задает тип 3D‑формы, используемый в 3D‑гистограмме или столбчатой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

Получает или задает тип 3D‑формы, используемой в 3‑D столбчатой или колонковой диаграмме.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
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

            // Добавить 3D‑гистограмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить тип формы столбца в Цилиндр
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Сохраните книгу
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


