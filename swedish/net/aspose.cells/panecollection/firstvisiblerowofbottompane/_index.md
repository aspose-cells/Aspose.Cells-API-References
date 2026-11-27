---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaneCollection-egenskap. Hämtar och anger den första synliga raden i den nedre panelen"
type: docs
url: /sv/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Hämtar och anger den första synliga raden i den nedre panelen.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa en rullningsbar panel
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Frys paneler på rad 10 (detta skapar övre och nedre paneler)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Hämta panelsamlingen
            PaneCollection panes = worksheet.GetPanes();
            
            // Ange den första synliga raden i den nedre panelen
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Skriv ut den första synliga raden i den nedre panelen
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Spara arbetsboken
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Se även

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


