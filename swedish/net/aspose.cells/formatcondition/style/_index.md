---
title: "FormatCondition.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämtar eller anger stil för villkorligt formaterade cellområden"
type: docs
url: /sv/net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Hämtar eller anger stil för villkorligt formaterade cellområden.

```csharp
public Style Style { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(30);
            worksheet.Cells["A2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(90);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ange intervallet
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            // Lägg till första villkoret (värden mellan 40‑80)
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
            fc1.Style.Font.Color = System.Drawing.Color.Black;

            // Lägg till andra villkoret (värden > 80)
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;
            fc2.Style.Font.Color = System.Drawing.Color.White;
            fc2.Style.Font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("FormatConditionStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


