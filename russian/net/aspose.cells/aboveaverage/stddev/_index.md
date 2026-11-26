---
title: "AboveAverage.StdDev"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AboveAverage. Получает или задает количество стандартных отклонений, которое следует включать выше или ниже среднего в правиле условного форматирования. Входное значение должно быть от 0 до 3 включительно. Установка значения 0 означает, что stdDev не задан. Значение по умолчанию равно 0."
type: docs
url: /ru/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Получить или задать количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. Входное значение должно быть от 0 до 3 (включительно). Установка значения 0 означает, что stdDev не задан. Значение по умолчанию — 0.

```csharp
public int StdDev { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Заполнить примерными данными
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### См. также

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


