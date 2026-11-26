---
title: "Bevel.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Bevel свойство. Получает и задает предустановленный тип фаски"
type: docs
url: /ru/net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Получает и задает тип предустановленной фаски.

```csharp
public BevelPresetType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Установить цвет серии
            series.Area.ForegroundColor = Color.Blue;

            // Настроить 3D-формат и свойства фаски
            Format3D format3D = series.ShapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            // Продемонстрировать использование свойства Type
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 5;
            topBevel.Height = 2;

            // Сохраните книгу
            workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


