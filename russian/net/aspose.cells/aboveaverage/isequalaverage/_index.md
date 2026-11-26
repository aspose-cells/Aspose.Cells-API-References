---
title: "AboveAverage.IsEqualAverage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AboveAverage. Получает или задает флаг, указывающий, включают ли критерии aboveAverage и belowAverage само среднее значение или исключают его. true означает включить среднее значение в критерий. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Получить или задать флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. Значение 'true' означает включить среднее значение в критерий. Значение по умолчанию — false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
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
            fc.Style.BackgroundColor = Color.LightBlue;

            // Продемонстрировать свойство IsEqualAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Заполнить примерными данными
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### См. также

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


