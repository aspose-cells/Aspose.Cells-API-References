---
title: "DataBar.MaxLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Representerar den maximala längden på en datastapel"
type: docs
url: /sv/net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

Representerar den maximala längden på en data bar.

```csharp
public int MaxLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsstyrd formatering
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            
            CellArea area = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(area);

            // Lägg till datastapel och ställ in egenskaper
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;
            
            dataBar.Color = Color.Blue;
            dataBar.MinLength = 0;
            dataBar.MaxLength = 90; // Demonstrating MaxLength property
            
            workbook.Save("DataBarMaxLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


