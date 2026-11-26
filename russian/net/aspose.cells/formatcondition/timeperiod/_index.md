---
title: "FormatCondition.TimePeriod"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Применимый период времени в условном правиле форматирования даты. Доступно только для типа timePeriod. Значение по умолчанию — TimePeriodType.Today."
type: docs
url: /ru/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

Применимый период времени в правиле условного форматирования "date occurrin". Действительно только для type = timePeriod. Значение по умолчанию — TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTimePeriodDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные даты для демонстрации форматирования по периоду времени
            worksheet.Cells["A1"].PutValue(DateTime.Now);
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
            fc.TimePeriod = TimePeriodType.Today;

            workbook.Save("TimePeriodDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


