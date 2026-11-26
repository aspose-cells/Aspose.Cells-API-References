---
title: "FormatCondition.TimePeriod"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. El período de tiempo aplicable en una regla de formato condicional de fecha. Válido solo para el tipo timePeriod. El valor predeterminado es TimePeriodType.Today"
type: docs
url: /es/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Ejemplos

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

            // Agregar valores de fecha de muestra para demostrar el formato de período de tiempo
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

### Ver también

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


