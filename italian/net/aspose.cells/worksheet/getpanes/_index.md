---
title: "Worksheet.GetPanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene i riquadri della finestra"
type: docs
url: /it/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Ottiene i riquadri della finestra.

```csharp
public PaneCollection GetPanes()
```

### Osservazioni

Se la finestra non è divisa o congelata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Congela i riquadri alla riga 5 e alla colonna 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Ottieni le informazioni del riquadro
            PaneCollection panes = worksheet.GetPanes();
            
            // Visualizza le informazioni del riquadro
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


