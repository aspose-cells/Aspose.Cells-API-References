---
title: "DataBar.MaxCfvo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämta eller ange detta DataBars maxvärdesobjekt. Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Min till det"
type: docs
url: /sv/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Hämta eller ange detta DataBars maxvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Min till det.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorlig formatering för datastaplar
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Lägg till datastapel
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // Ange MaxCfvo-värde
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Spara arbetsboken
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


