---
title: "Worksheet.GetPanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Hämtar fönsterpanelerna"
type: docs
url: /sv/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Hämtar fönsterpanelerna.

```csharp
public PaneCollection GetPanes()
```

### Anmärkningar

Om fönstret inte är delat eller fryst.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Frys paneler vid rad 5 och kolumn 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Hämta panelinformation
            PaneCollection panes = worksheet.GetPanes();
            
            // Visa panelinformation
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


