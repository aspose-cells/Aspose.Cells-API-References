---
title: "DataBar.MinLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Representerar minlängden för datastapeln"
type: docs
url: /sv/net/aspose.cells/databar/minlength/
---
## DataBar.MinLength property

Representerar den minsta längden på en data bar.

```csharp
public int MinLength { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["A4"].PutValue(35);

            // Lägg till villkorsstyrd formatering
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

            // Lägg till datastapel
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            DataBar dataBar = fc.DataBar;

            // Konfigurera datastapel
            dataBar.Color = Color.Green;
            dataBar.MinLength = 10;  // Minimum length set to 10%
            dataBar.MaxLength = 100;

            workbook.Save("DataBarMinLengthDemo.xlsx");
            Console.WriteLine("DataBar with MinLength demo executed successfully.");
        }
    }
}
```

### Se även

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


