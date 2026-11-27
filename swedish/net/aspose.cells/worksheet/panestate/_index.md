---
title: "Worksheet.PaneState"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om panelen har horisontella eller vertikala delningar och om dessa delningar är frysta"
type: docs
url: /sv/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Anger om panelen har horisontella eller vertikala delningar, och om dessa delningar är frysta.

```csharp
public PaneStateType PaneState { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Frys paneler (första raden)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Hämta och visa panelens tillstånd
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Spara arbetsbok
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


