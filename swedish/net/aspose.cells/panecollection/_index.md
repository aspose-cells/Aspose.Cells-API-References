---
title: "Klass PaneCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PaneCollection-klass. Representerar alla Pane-objekt som visas i det angivna fönstret"
type: docs
url: /sv/net/aspose.cells/panecollection/
---
## PaneCollection class

Representerar alla Pane-objekt som visas i det angivna fönstret.

```csharp
public class PaneCollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) Hämtar och anger den aktiva panelen. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Hämtar och anger den aktiva panelen. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Hämtar och anger den första synliga kolumnen i den högra panelen. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Hämtar och anger den första synliga raden i den nedre panelen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Frys paneler på rad 5, kolumn 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Hämta panelsamling
            PaneCollection panes = sheet.GetPanes();
            
            // Ändra panelinställningar
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Spara arbetsboken
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


