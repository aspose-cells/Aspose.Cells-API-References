---
title: "DataBar.AxisPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar property. Hämtar eller anger positionen för axeln på datastaplarna som specificeras av en villkorsstyrd formateringsregel"
type: docs
url: /sv/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Hämtar eller anger positionen för axeln på data bars som specificeras av en villkorsstyrd formateringsregel.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Lägg till villkorlig formatering för datastaplar
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            
            // Konfigurera datastapelns egenskaper
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // Ställ in axelposition (grundläggande demonstration)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // Spara arbetsboken
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### Se även

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


