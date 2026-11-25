---
title: "NegativeBarFormat.BorderColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NegativeBarFormat. Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore del bordo per le barre dati negative"
type: docs
url: /it/net/aspose.cells/negativebarformat/bordercolor/
---
## NegativeBarFormat.BorderColor property

Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore del bordo per le barre dati negative.

```csharp
public Color BorderColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];
            DataBar dataBar = cond.DataBar;

            dataBar.Color = Color.Orange;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            sheet.Cells["A1"].PutValue(-10);
            sheet.Cells["A2"].PutValue(50);
            sheet.Cells["A3"].PutValue(-100);

            workbook.Save("NegativeBarFormatBorderColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


