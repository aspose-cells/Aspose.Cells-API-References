---
title: "FormatCondition.TimePeriod"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Il periodo di tempo applicabile in una regola di formattazione condizionale basata su data. Valido solo per il tipo timePeriod. Il valore predefinito è TimePeriodType.Today"
type: docs
url: /it/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

Il periodo di tempo applicabile in una regola di formattazione condizionale "date occurrin". Valida solo per type = timePeriod. Il valore predefinito è TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Esempi

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

            // Aggiungi valori di data di esempio per dimostrare la formattazione del periodo di tempo
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

### Vedi anche

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


