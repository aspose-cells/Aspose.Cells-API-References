---
title: "Worksheet.PaneState"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate"
type: docs
url: /it/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate.

```csharp
public PaneStateType PaneState { get; }
```

### Esempi

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

            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Blocca i riquadri (prima riga)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Ottieni e visualizza lo stato del riquadro
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Salva cartella di lavoro
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


