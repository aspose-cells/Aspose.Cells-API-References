---
title: "FormatCondition.TimePeriod"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Den tillämpliga tidsperioden i ett datum som förekommer i en villkorlig formateringsregel. Giltig endast för typen timePeriod. Standardvärdet är TimePeriodType.Today"
type: docs
url: /sv/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

Den tillämpliga tidsperioden i en "date occurrin"-villkorlig formateringsregel. Giltig endast för typ = timePeriod. Standardvärdet är TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Exempel

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

            // Lägg till exempelvärden för datum för att demonstrera tidsperiodformatering
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

### Se även

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


