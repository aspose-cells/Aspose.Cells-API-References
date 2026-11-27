---
title: "FormatCondition.DataBar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämta den villkorliga formaterings‑DataBar‑instansen. Standardinstansens färg är blå. Giltig endast för typen DataBar."
type: docs
url: /sv/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Hämta den villkorliga formateringens "DataBar"-instans. Standardinstansens färg är blå. Giltig endast för typ = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Lägg till villkorlig formatering för datastaplar
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Ange intervallet för villkorlig formatering
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Lägg till datafältvillkor och ange egenskaper
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Konfigurera DataBar-egenskaper
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Spara arbetsboken
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Se även

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


