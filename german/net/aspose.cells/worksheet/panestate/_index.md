---
title: "Worksheet.PaneState"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob das Fenster horizontale oder vertikale Teilungen hat und ob diese Teilungen eingefroren sind"
type: docs
url: /de/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Gibt an, ob das Fenster horizontale oder vertikale Teilungen hat und ob diese Teilungen eingefroren sind.

```csharp
public PaneStateType PaneState { get; }
```

### Beispiele

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

            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Fenster einfrieren (erste Zeile)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Fensterstatus abrufen und anzeigen.
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Arbeitsmappe speichern.
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


