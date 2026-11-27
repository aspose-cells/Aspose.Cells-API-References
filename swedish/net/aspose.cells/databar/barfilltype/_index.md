---
title: "DataBar.BarFillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämtar eller anger hur en datastapel fylls med färg"
type: docs
url: /sv/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Hämtar eller anger hur en data bar fylls med färg.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Instansiera ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ange området för villkorsformatering
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // Lägg till DataBar-villkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Konfigurera DataBar-egenskaper
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Spara arbetsboken
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


