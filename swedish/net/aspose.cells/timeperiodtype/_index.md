---
title: "Enum TimePeriodType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TimePeriodType-enum. Används i en FormatConditionType.TimePeriod-regel för villkorsstyrd formatering. Detta är dynamiska tidsperioder som förändras baserat på datumet då den villkorsstyrda formateringen uppdateras / tillämpas"
type: docs
url: /sv/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Används i en FormatConditionType.TimePeriod‑regel för villkorsstyrd formatering. Detta är dynamiska tidsperioder som förändras baserat på datumet då den villkorsstyrda formateringen uppdateras/tillämpas.

```csharp
public enum TimePeriodType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Today | `0` | Dagens datum. |
| Yesterday | `1` | Gårdagens datum. |
| Tomorrow | `2` | Morgondagens datum. |
| Last7Days | `3` | Ett datum under de senaste sju dagarna. |
| ThisMonth | `4` | Ett datum som inträffar i denna kalendermånad. |
| LastMonth | `5` | Ett datum som inträffar under den senaste kalendermånaden. |
| NextMonth | `6` | Ett datum som inträffar under nästa kalendermånad. |
| ThisWeek | `7` | Ett datum som inträffar den här veckan. |
| LastWeek | `8` | Ett datum som inträffar förra veckan. |
| NextWeek | `9` | Ett datum som inträffar nästa vecka. |
| ThisYear | `10` | Ett datum som inträffar i år. Endast för .ods. |
| LastYear | `11` | Ett datum som inträffar förra året. Endast för .ods. |
| NextYear | `12` | Ett datum som inträffar nästa år. Endast för .ods. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en regel för villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definiera cellområdet för den villkorsstyrda formateringen
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Lägg till ett villkor för tidsperioden
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Ange typ av tidsperiod
            fc.TimePeriod = TimePeriodType.Today;

            // Spara arbetsboken
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


