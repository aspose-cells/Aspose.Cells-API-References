---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaneCollection-egenskap. Hämtar och anger den första synliga kolumnen i den högra panelen"
type: docs
url: /sv/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Hämtar och anger den första synliga kolumnen i den högra panelen.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Frys paneler genom att ange rad- och kolumnindex (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Hämta panelsamlingen
            PaneCollection panes = sheet.GetPanes();
            
            // Ställ in den första synliga kolumnen i den högra panelen
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


