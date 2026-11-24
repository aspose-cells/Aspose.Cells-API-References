---
title: "Worksheet.IsRulerVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur in der Seitenumbruchvorschau angewendet"
type: docs
url: /de/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur für die Seitenumbruchvorschau angewendet.

```csharp
public bool IsRulerVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze das Arbeitsblatt auf PageLayoutView, bei dem das Lineal sichtbar ist.
            worksheet.ViewType = ViewType.PageLayoutView;

            // Linealsichtbarkeit umschalten
            worksheet.IsRulerVisible = true;

            // Gib den aktuellen Zustand der Linealsichtbarkeit aus
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


