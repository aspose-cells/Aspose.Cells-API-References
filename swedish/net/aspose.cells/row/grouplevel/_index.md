---
title: "Row.GroupLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar gruppnivån för raden"
type: docs
url: /sv/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Hämtar gruppnivån för raden.

```csharp
public byte GroupLevel { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppera rader 4-6 (hidden = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Åtkomst till gruppnivån för rad 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Avgruppera raderna
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


