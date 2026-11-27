---
title: "DataBar.MinCfvo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämta eller ange detta DataBars minsta värdeobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det"
type: docs
url: /sv/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Hämta eller ange detta DataBars minvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Hämta den villkorsstyrda formateringssamlingen
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Skapa en datastapel med MinCfvo inställd på typen \"Value\"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Ange datastapelsintervallet
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Spara arbetsboken
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


