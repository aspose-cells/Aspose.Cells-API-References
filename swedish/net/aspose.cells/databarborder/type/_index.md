---
title: "DataBarBorder.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBarBorder-egenskap. Hämtar eller anger kantens typ för datastaplar som specificeras av en villkorsstyrd formateringsregel"
type: docs
url: /sv/net/aspose.cells/databarborder/type/
---
## DataBarBorder.Type property

Hämtar eller anger kantens typ på datastaplarna som specificeras av en villkorsstyrd formateringsregel.

```csharp
public DataBarBorderType Type { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            DataBar dataBar = fc.DataBar;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Red;

            workbook.Save("DataBarBorderTypeExample.xlsx");
        }
    }
}
```

### Se även

* enum [DataBarBorderType](../../databarbordertype/)
* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


